<template lang="html">
  <div id="info-box" v-if='country'>
    <h3>{{country.name}}</h3>
    <img class="flag" :src='country.flag'/>
    <p>Capital: {{country.capital}}</p>
    <p>Population: {{country.population}}</p>
    <!-- <p v-for="language in country.languages">Languages: {{countries.languages.name}}</p> -->
  </div>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country', 'countries']
}
</script>

<style lang="css" scoped>
 #info-box {
   border: solid 2px black;
   border-radius: 10px;
   padding: 10px;
   position: fixed;
   top: 100px;
   right: 100px;
 }

.flag {
  width: 120px;
}
</style>
