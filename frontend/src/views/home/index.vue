<script>
import Post from '@/components/Post.vue'
export default {
  name:"Home",
  components:{
    Post
  }
}
</script>

<template lang="pug">
.home
  .timeline
    Post
    br
    Post
    br
    Post
    br
    Post
    br
    Post
    br
  .sidebar

</template>

<style scoped>
.home {
  display: grid;
  grid-template-columns: 1fr 295px;
  grid-gap: 30px;
}

</style>