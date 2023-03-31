<template>
    <section class="AboutMeContainer">
        <div class="AboutMeContent">
            <SectionHeader title="Who Am I" />
            <section class="QuoteContainer">
                <!-- <h2>Runner. Trumpet player. Programmer.</h2> -->
                <!-- <h3>🏃🎺💻</h3> -->
            </section>
            <section class="PhotoContainer">
                <img src="/TrumpetHeadshot.jpg" />
                <img src="/TrumpetHeadshot.jpg" />
                <img src="/TrumpetHeadshot.jpg" />
            </section>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import SectionHeader from './SectionHeader.vue';

export default defineComponent({
    name: "AboutMe",
    components: {
        SectionHeader
    }
});
</script>

<style lang="scss" scoped>
section.AboutMeContainer {
    margin: 100px 0;

    .AboutMeContent {
        margin: auto;
        width: 75%;
    }

    .QuoteContainer {
        text-align: center;
        margin-top: 100px;

        h2 {
            font-size: 2.25rem;
            letter-spacing: 0.5rem;
            font-weight: 200;
            margin-bottom: 75px;
            opacity: 0.55;
        }

        /*
        h3 {
            font-size: 2.5rem;
            letter-spacing: 4rem;
            margin-bottom: 100px;
        } */
    }

    .PhotoContainer {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 30px;

        img {
            border-radius: 15px;
            box-shadow: rgba(0, 0, 0, 0.5) 0px 3px 6px, rgba(0, 0, 0, 0.23) 0px 3px 6px;
            transition: transform 200ms ease-in;
            cursor: pointer;
        }

        img:hover {
            transform: scale(1.05);
        }
    }
}
</style>
