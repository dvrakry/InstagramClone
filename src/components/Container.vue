<template>
  <div>
      <Post :인스타데이터="인스타데이터[i]" v-for="(a,i) in 인스타데이터" :key="i"/>
      <!-- <Post :인스타데이터="인스타데이터[1]"/>
      <Post :인스타데이터="인스타데이터[2]"/> -->
  </div>
</template>

<script>

import Post from './Post.vue'

export default {
    components : {
        Post : Post,
    },
    props:{
        인스타데이터 : Array,
    },
}
</script>

<style>

</style>