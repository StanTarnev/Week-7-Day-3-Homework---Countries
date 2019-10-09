<template lang="html">
  <ul>
    <list-component v-for="(country, index) in countries" :country="country" :key="index">{{country.name}}</list-component>
  </ul>

</template>

<script>
import ListComponent from './ListComponent.vue';

export default {
  name: 'countries-list',
  props: ['countries'],
  components: {
    'list-component': ListComponent
  }
}
</script>

<style lang="css" scoped>
</style>
