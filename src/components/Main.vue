<template>
  <main>
    <OurPeople />
    <OurValues />
    <RecentCauses />
  </main>
</template>

<script>
  import OurPeople from './MainSections/OurPeople.vue';
  import OurValues from './MainSections/OurValues.vue';
  import RecentCauses from './MainSections/RecentCauses.vue';

  export default {
    name: 'Main',
    components: {
      OurPeople,
      OurValues,
      RecentCauses
    }
  }
</script>

<style lang="scss">
</style>