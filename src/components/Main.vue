<template>
  <main>
    <OurPeople />
    <OurValues />
    <RecentCauses />
    <LatestArticles />
  </main>
</template>

<script>
  import OurPeople from './MainSections/OurPeople.vue';
  import OurValues from './MainSections/OurValues.vue';
  import RecentCauses from './MainSections/RecentCauses.vue';
  import LatestArticles from './MainSections/LatestArticles.vue';

  export default {
    name: 'Main',
    components: {
      OurPeople,
      OurValues,
      RecentCauses,
      LatestArticles
    }
  }
</script>

<style lang="scss">
</style>