<template>
  <ul class="collection">
    <li class="collection-item avatar" v-for="(characters, index) in characters" :key ="index">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcStsRIcYrDBwub9OR7q2_n__1xswyMk8mn4hMi0oSPAhbyqSxP0" alt="" class="circle">
      <span class="title">{{ characters.name }}</span>
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    characters: Array
  }
};
</script>

<style>
</style>
