<template>
  <main>
    <OurPeople />
    <OurValues />
  </main>
</template>

<script>
  import OurPeople from './MainSections/OurPeople.vue';
  import OurValues from './MainSections/OurValues.vue';

  export default {
    name: 'Main',
    components: {
      OurPeople,
      OurValues
    }
  }
</script>

<style lang="scss">
</style>