<script>
import CustomText from '@/components/CustomText.vue'
import HomeIcon from '@/icons/home.svg'

export default {
  name:"Home",
  components:{
    CustomText,
    HomeIcon
  }
}
</script>

<template lang="pug">
div
  CustomText Hello World
  CustomText(tag="p" class="a1") Hello World
  CustomText(tag="p" class="a2" size="small") Hello World
  CustomText(tag="p" class="a3" size="xsmall") Hello World
  CustomText(tag="p" class="a4" size="xxsmall") Hello World
  HomeIcon(width="60" height="60")
</template>

<style scoped>
.a1{
  color: rgb(var(--ba8));
}
.a2{
  color: rgb(var(--eac));
}
.a3{
  color: rgb(var(--fa7));
}
.a4{
  color: rgb(var(--d20));
}
</style>