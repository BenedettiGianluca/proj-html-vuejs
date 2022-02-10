<template>
  <main>
    <OurPeople />
    <OurValues />
    <RecentCauses />
    <LatestArticles />
    <ChangeToday />
  </main>
</template>

<script>
  import OurPeople from './MainSections/OurPeople.vue';
  import OurValues from './MainSections/OurValues.vue';
  import RecentCauses from './MainSections/RecentCauses.vue';
  import LatestArticles from './MainSections/LatestArticles.vue';
  import ChangeToday from './MainSections/ChangeToday.vue';

  export default {
    name: 'Main',
    components: {
      OurPeople,
      OurValues,
      RecentCauses,
      LatestArticles,
      ChangeToday
    }
  }
</script>

<style lang="scss">
</style>