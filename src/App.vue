<script lang="ts">
import { defineComponent } from "vue";

import NavigationMenu from "./components/NavigationMenu.vue";
import IntroContent from "./components/IntroContent.vue";
import AboutMe from "./components/AboutMe.vue";
import ProjectSection from "./components/ProjectSection.vue";

export default defineComponent({
  components: {
    NavigationMenu,
    IntroContent,
    AboutMe,
    ProjectSection
}
})
</script>

<template>
  <NavigationMenu></NavigationMenu>
  <IntroContent></IntroContent>
  <AboutMe></AboutMe>
  <ProjectSection></ProjectSection>
</template>

<style lang="scss" scoped>

</style>
