<script>
import Header from '@/components/Header.vue'
import Container from '@/components/Container.vue'


export default {
  components:{
    Header,
    Container
  }
}
</script>

<template lang="pug">
#app
  Header
  main.content
    Container
      router-view
</template>

<style lang="scss" scoped>
.content {
 padding-top: 40px;
}
</style>