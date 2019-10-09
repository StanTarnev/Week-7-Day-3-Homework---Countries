<template lang="html">
  <div id="info-box" v-if='country'>
    <h3>{{country.name}}</h3>
    <p>Capital: {{country.capital}}</p>
    <p>Population: {{country.population}}</p>
  </div>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style lang="css" scoped>
 #info-box {
   border: solid 2px black;
   border-radius: 5px;
   padding: 10px;
   position: fixed;
   top: 100px;
   right: 100px;

 }
</style>
