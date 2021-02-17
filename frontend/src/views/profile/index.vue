<script>
import CustomText from '@/components/CustomText.vue'

export default {
  name: "Profile",
  components:{
      CustomText
  }
}
</script>

<template lang="pug">
div
  CustomText(tag="h1") Profile Page
  div
    router-link(to="/profile") Post |
    router-link(to="/profile/igtv") Igtv |
    router-link(to="/profile/save") Save |
    router-link(to="/profile/tag") Tag

  router-view
</template>

<style lang="scss" scoped>

</style>