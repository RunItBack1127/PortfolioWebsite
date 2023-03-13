<template>
    <header>
        <section class="HomeContainer">
            <div class="ContactInformation">
                <a href="https://linkedin.com/in/wpgreene" target="_blank">
                    <svg fill="#000000" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 310 310" xml:space="preserve">
                        <g id="XMLID_801_">
                            <path id="XMLID_802_" d="M72.16,99.73H9.927c-2.762,0-5,2.239-5,5v199.928c0,2.762,2.238,5,5,5H72.16c2.762,0,5-2.238,5-5V104.73   C77.16,101.969,74.922,99.73,72.16,99.73z"/>
                            <path id="XMLID_803_" d="M41.066,0.341C18.422,0.341,0,18.743,0,41.362C0,63.991,18.422,82.4,41.066,82.4   c22.626,0,41.033-18.41,41.033-41.038C82.1,18.743,63.692,0.341,41.066,0.341z"/>
                            <path id="XMLID_804_" d="M230.454,94.761c-24.995,0-43.472,10.745-54.679,22.954V104.73c0-2.761-2.238-5-5-5h-59.599   c-2.762,0-5,2.239-5,5v199.928c0,2.762,2.238,5,5,5h62.097c2.762,0,5-2.238,5-5v-98.918c0-33.333,9.054-46.319,32.29-46.319   c25.306,0,27.317,20.818,27.317,48.034v97.204c0,2.762,2.238,5,5,5H305c2.762,0,5-2.238,5-5V194.995   C310,145.43,300.549,94.761,230.454,94.761z"/>
                        </g>
                    </svg>
                </a>
                <a href="https://github.com/RunItBack1127" target="_blank">
                    <svg fill="#000000" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path></svg>
                    <!-- <svg viewBox="0 0 1920 1920" xmlns="http://www.w3.org/2000/svg">
                        <path d="M1821.63 637.76c0-130.027-43.627-236.373-116.054-319.68 11.627-30.187 50.347-151.36-11.2-315.307 0 0-94.72-32-310.4 122.134-90.133-26.454-186.773-39.68-282.773-40.107-96 .427-192.64 13.653-282.667 40.107C602.749-29.227 507.923 2.773 507.923 2.773c-61.547 163.947-22.72 285.12-11.094 315.307-72.32 83.307-116.266 189.653-116.266 319.68 0 456.533 263.68 558.72 514.453 588.8 0 0-180.267 111.68-180.267 299.413-64.32 30.507-336.533 123.947-437.333-58.133 0 0-59.627-114.347-173.013-122.773 0 0-110.294-1.494-7.787 72.426 0 0 74.027 36.694 125.44 174.294 0 0 57.173 289.92 489.067 159.68 4.373 2.24 1.6 140.266 1.6 168.533h777.173s1.28-277.013 1.28-365.12c0-216.64-144.64-292.48-185.28-329.28 251.627-29.44 515.733-130.133 515.733-587.84" fill-rule="evenodd"/>
                    </svg> -->
                </a>
                <button>
                    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g id="style=linear">
                            <g id="email">
                                <path id="vector" d="M17 20.5H7C4 20.5 2 19 2 15.5V8.5C2 5 4 3.5 7 3.5H17C20 3.5 22 5 22 8.5V15.5C22 19 20 20.5 17 20.5Z" stroke="#000000" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                                <path id="vector_2" d="M18.7698 7.7688L13.2228 12.0551C12.5025 12.6116 11.4973 12.6116 10.777 12.0551L5.22998 7.7688" stroke="#000000" stroke-width="1.5" stroke-linecap="round"/>
                            </g>
                        </g>
                    </svg>
                </button>
            </div>
            <nav>
                <MenuOption :optionDisabled="true" name="Home"></MenuOption>
                <MenuOption name="Who Am I"></MenuOption>
                <MenuOption name="My Projects"></MenuOption>
                <button id="ContactInfo">Contact Me</button>
            </nav>
        </section>
    </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import MenuOption from './MenuOption.vue';

export default defineComponent({
    name: 'NavigationMenu',
    components: {
        MenuOption
    }
});
</script>

<style lang="scss" scoped>
header {
    width: 100%;

    section {
        width: 75%;
        height: 120px;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .ContactInformation {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 0 50px;

            a, button {
                width: 30px;

                svg {
                    width: 27.5px;
                    height: 27.5px;
                }
            }

            a:hover, button:hover {
                opacity: 0.8;
            }
        }

        nav {
            display: flex;
            justify-content: center;
            align-items: center;

            button {
                font-size: 1.35rem;
                letter-spacing: 0.1rem;
                padding: 20px;
            }

            button:not(:last-child) {
                margin-right: 45px;
            }

            button#ContactInfo {
                background: #000;
                color: #fff;
                font-weight: 600;
                padding: 15px 35px;
                border-radius: 10px;
            }
        }
    }
}
</style>