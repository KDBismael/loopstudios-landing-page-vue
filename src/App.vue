<script>
  import heroSection from "./components/hero-section.vue";
  import heroContent from "./components/hero-content.vue";
  import expertiseSection from "./components/expertise-section.vue";
  import creationSection from "./components/creation-section.vue";
  import appFooter from "./components/app-footer.vue";
import AppFooter from "./components/app-footer.vue";

  export default{
    components:{
    heroSection,
    heroContent,
    expertiseSection,
    creationSection,
    appFooter,
    AppFooter
}
  }
</script>

<template>
  <div>
    <hero-section>
      <template v-slot:default>
        <hero-content content="Immersive experiences that deliver"></hero-content>
      </template>
    </hero-section>
    <expertise-section  />
    <creation-section/>
    <app-footer/>
  </div>
</template>

<style>

</style>
