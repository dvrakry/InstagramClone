<template>
  <div>
      <Post :게시물="게시물[i]" v-for="(a,i) in 게시물" :key="i"/>
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
        게시물 : Array,
    },
}
</script>

<style>

</style>