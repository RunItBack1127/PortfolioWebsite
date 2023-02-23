<script lang="ts">
import { defineComponent } from "vue";

import NavigationMenu from "./components/NavigationMenu.vue";
import IntroContent from "./components/IntroContent.vue";
import AboutMe from "./components/AboutMe.vue";

export default defineComponent({
  components: {
    NavigationMenu,
    IntroContent,
    AboutMe
  }
})
</script>

<template>
  <NavigationMenu></NavigationMenu>
  <IntroContent></IntroContent>
  <AboutMe></AboutMe>
</template>

<style lang="scss" scoped>

</style>
