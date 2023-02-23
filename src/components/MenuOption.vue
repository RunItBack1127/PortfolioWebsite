<template>
    <div class="MenuOption" :class="optionDisabled ? 'currentTab' : ''">
        <button :disabled="optionDisabled" @click="navigate()">{{ name }}</button>
        <span :class="optionDisabled ? 'optionDisabled' : ''"></span>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'MenuOption',
    props: {
        name: String,
        navigateTo: Function,
        optionDisabled: Boolean
    },
    methods: {
        navigate: function() {
            if( this.navigateTo ) {
                this.navigateTo();
            }
        }
    }
})
</script>

<style lang="scss" scoped>
    .MenuOption {
        box-sizing: content-box;
        display: flex;
        flex-direction: column;
        margin-right: 60px;

        button {
            display: flex;
            flex-direction: column;
            text-align: center;
            font-size: 1.25rem;
            letter-spacing: 0.1rem;
            padding: 15px 5px;
        }

        button:disabled {
            pointer-events: none;
            opacity: 0.9;
        }

        span {
            display: block;
            bottom: -5px;
            width: 100%;
            height: 1px;
            background: linear-gradient(to right, #000, #000);
            background-repeat: no-repeat;
            background-size: 0 100%;
            transition: background-size 65ms ease;
        }

        span.optionDisabled {
            opacity: 0.25;
        }
    }

    .MenuOption.currentTab {

        span {
            background-size: 100% 100%;
        }
    }

    .MenuOption:hover {

        span {
            background-size: 100% 100%;
        }
    }
</style>