<template>
    <section class="IntroContainer">
        <div class="IntroContent">
            <div class="TextContainer">
                <h1>Hi, I'm Weston! <span>👋</span></h1>
                <h2>I'm an experienced full-stack developer based in the Research Triangle Park. Yes, I can fix your printer.</h2>
                <nav>
                    <button>About Me</button>
                    <button id="ContactInfo">Let's Connect!</button>
                </nav>
            </div>
            <div class="PhotoContent">
                <div class="PhotoContainer">
                    <img src="/SiteHeadshot.jpg" />
                </div>
            </div>
        </div>
        <!-- <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#111111" fill-opacity="1" d="M0,32L80,26.7C160,21,320,11,480,48C640,85,800,171,960,181.3C1120,192,1280,128,1360,96L1440,64L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"></path></svg>    
     -->
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'IntroContent',
});
</script>

<style lang="scss" scoped>
section {
    position: relative;
    width: 100%;

    .IntroContent {
        width: 75%;
        margin: auto;
        display: grid;
        grid-template-columns: 1fr 1fr;

        .TextContainer {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            
            h1 {
                font-family: 'Coolvetica', sans-serif;
                font-size: 5rem;
                margin-bottom: 20px;

                span {
                    display: inline-block;
                    font-size: 0.5em;
                    transform: translateY(-25%);
                }
            }

            h2 {
                font-size: 2rem;
                font-weight: 100;
                letter-spacing: 0.1rem;
                line-height: 2.5rem;
                margin-bottom: 60px;
            }

            nav {
                display: flex;

                button {
                    font-size: 1.75rem;
                    text-align: center;
                }

                button:first-child {
                    margin-right: 50px;
                    border-bottom: 1px solid rgba(0, 0, 0, 0.5);
                }

                button#ContactInfo {
                    padding: 20px 50px;
                    border-radius: 10px;
                    background: #000;
                    color: #fff;
                }
            }
        }

        .PhotoContent {
            display: flex;
            justify-content: center;
            align-items: center;

            .PhotoContainer {
                filter: drop-shadow(rgba(0, 0, 0, 0.2) 0px 3px 20px);

                img {
                    width: 450px;
                    clip-path: circle();
                }
            }
        }
    }
}
</style>