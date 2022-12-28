<template>
<div v-for="(a,i) in data" :key="i">
  <h5 @click="$router.push(`/detail/${i}`)"> {{data[i].title}}</h5>
  <p>{{data[i]}}</p>
  <p>{{data[i].content}}</p>
</div>
</template>

<script>
export default {
  name: "TheList",
  props:{
    data:Array,
  }
}
</script>

<style scoped>

</style>