<template>
    <div class="SectionHeaderContainer">
        <h1>{{ title }}</h1>
        <div class="UnderlineContainer">
            <span></span>
            <span></span>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'SectionHeader',
    props: {
        title: String
    }
})
</script>

<style lang="scss">
.SectionHeaderContainer {
    width: 100%;
    text-align: center;

    h1 {
        font-size: 3rem;
        font-weight: 100;
        letter-spacing: 0.25rem;
        margin-bottom: 20px;
    }

    .UnderlineContainer {
        width: 100%;
        display: grid;
        grid-template-columns: 30% 70%;
        
        span {
            background: #000;
            height: 1px;
        }

        span:last-child {
            opacity: 0.25;
        }
    }
}
</style>