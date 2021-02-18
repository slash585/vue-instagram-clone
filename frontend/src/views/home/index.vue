<script>
import CustomText from '@/components/CustomText.vue'

export default {
  name:"Home",
  components:{
  }
}
</script>

<template lang="pug">
.home
  .timeline
  .sidebar

</template>

<style scoped>
.home {
  display: grid;
  grid-template-columns: 1fr 295px;
  grid-gap: 30px;
}

</style>