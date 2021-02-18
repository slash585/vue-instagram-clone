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
.home
  .timeline
    p Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id risus diam. Vivamus bibendum augue vitae est gravida, ut pretium mi porttitor. Ut tincidunt mollis est, quis ornare odio aliquam et. Praesent vitae justo auctor, fringilla lacus eu, pretium tortor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam suscipit dui sed arcu lacinia, in pulvinar ipsum gravida. Phasellus tristique diam ac arcu condimentum sodales. Vestibulum cursus tincidunt urna ac vestibulum. Nam iaculis ligula in mattis luctus.
    p Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id risus diam. Vivamus bibendum augue vitae est gravida, ut pretium mi porttitor. Ut tincidunt mollis est, quis ornare odio aliquam et. Praesent vitae justo auctor, fringilla lacus eu, pretium tortor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam suscipit dui sed arcu lacinia, in pulvinar ipsum gravida. Phasellus tristique diam ac arcu condimentum sodales. Vestibulum cursus tincidunt urna ac vestibulum. Nam iaculis ligula in mattis luctus.
    p Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id risus diam. Vivamus bibendum augue vitae est gravida, ut pretium mi porttitor. Ut tincidunt mollis est, quis ornare odio aliquam et. Praesent vitae justo auctor, fringilla lacus eu, pretium tortor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam suscipit dui sed arcu lacinia, in pulvinar ipsum gravida. Phasellus tristique diam ac arcu condimentum sodales. Vestibulum cursus tincidunt urna ac vestibulum. Nam iaculis ligula in mattis luctus.
  .sidebar
    p Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas id risus diam. Vivamus bibendum augue vitae est gravida, ut pretium mi porttitor. Ut tincidunt mollis est, quis ornare odio aliquam et. Praesent vitae justo auctor, fringilla lacus eu, pretium tortor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam suscipit dui sed arcu lacinia, in pulvinar ipsum gravida. Phasellus tristique diam ac arcu condimentum sodales. Vestibulum cursus tincidunt urna ac vestibulum. Nam iaculis ligula in mattis luctus.
</template>

<style scoped>
.home {
  display: grid;
  grid-template-columns: 1fr 295px;
  grid-gap: 30px;
}

</style>