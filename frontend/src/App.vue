<script>
export default {

}
</script>

<template lang="pug">
div
  div
    router-link(to="/") Home |
    router-link(to="/profile") Profile |
    router-link(to="/direct") Direct |
    router-link(to="/explore") Explore
  router-view
</template>

<style lang="scss" scoped>

</style>