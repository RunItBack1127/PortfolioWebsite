<template>
    <section class="IntroContainer">
        <div class="IntroContent">
            <div class="TextContainer">
                <h1>Hi, I'm Weston!</h1>
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
        <aside>
            <button>
                <svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 96 960 960" width="48"><path d="M480 712 240 472l43-43 197 197 197-197 43 43-240 240Z"/></svg>
            </button>
        </aside>
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
        grid-template-columns: 1fr 450px;
        gap: 150px;
        transform: translateY(-25px);

        .TextContainer {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            max-width: 600px;
            
            h1 {
                position: relative;
                font-family: 'Coolvetica', sans-serif;
                font-size: 5rem;
                margin-bottom: 20px;

                // span {
                //     display: inline-block;
                //     font-size: 0.5em;
                //     transform: translateY(-25%);
                // }
            }

            h1::after {
                content: '👋';
                position: absolute;
                font-size: 0.5em;
                top: 25%;
                transform: translateX(20px);
            }

            h2 {
                font-size: 1.75rem;
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

    aside {
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        bottom: 50px;

        button {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            box-shadow: rgba(0, 0, 0, 0.25) 0px 3px 8px;
            transition: transform 200ms ease;

            svg {
                opacity: 0.5;
                pointer-events: none;
            }
        }

        button:hover {
            transform: translateY(15px);
        }
    }
}
</style>