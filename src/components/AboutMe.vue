<template>
    <section class="AboutMeContainer">
        <aside>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#000000" fill-opacity="1" d="M0,96L80,117.3C160,139,320,181,480,186.7C640,192,800,160,960,144C1120,128,1280,128,1360,128L1440,128L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"></path></svg>
        </aside>
        <section class="AboutMeContent">
            <div class="AboutContent">
                <div class="PhotoContent">
                    <div class="PhotoContainer">
                        <img src="/TrumpetHeadshot.jpg" />
                    </div>
                </div>
                <div class="DescriptionContainer">
                    <h1>About Me</h1>
                    <p>I taught myself how to type, and it got out of control from there. I'm a developer that loves to learn new technologies and build software that people would want to use!</p>
                    <br>
                    <p>Outside of software, I'm a trumpet player and love to make music with other people. I also love to bike and lift weights, and of course, program (as a hobby! 😉)</p>
                </div>
            </div>
        </section>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'AboutMe'
});
</script>

<style lang="scss" scoped>

    section.AboutMeContainer {
        margin-top: -200px;

        section.AboutMeContent {
            width: 100%;
            background: #000;

            .AboutContent {
                margin: -150px auto auto;
                width: 80%;
                display: grid;
                grid-template-columns: 1fr 1fr;
                gap: 0 150px;

                .DescriptionContainer {
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: flex-start;
                    color: #fff;

                    h1 {
                        font-family: 'Coolvetica', sans-serif;
                        font-size: 4rem;
                        margin-bottom: 40px;
                    }

                    p {
                        font-size: 1.5rem;
                        line-height: 1.4em;
                    }

                    p:not(:last-child) {
                        margin-bottom: 30px;
                    }
                }
            }

            .PhotoContent {
                display: flex;
                justify-content: center;
                align-items: center;

                .PhotoContainer {
                    filter: drop-shadow(rgba(255, 255, 255, 0.2) 0px 3px 20px);

                    img {
                        width: 450px;
                        clip-path: circle();
                    }
                }
            }
        }

        aside {
            display: block;
            width: 100%;
            transform: scaleX(-1);
        }
    }
</style>