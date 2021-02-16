<script>
export default {
  name: 'CustomText',
  props: {
    tag: {
      type: String,
      default: 'span'
    },
    size: {
      type: String,
      default: 'normal',
      validator: function(value) {
        return ['normal', 'small', 'xsmall', 'xxsmall'].indexOf(value) !== -1
      }
    }
  }
}
</script>

<template lang="pug">
component(:is='tag' :class='size')
  slot
</template>

<style scoped>
.small {
    font-size: 12px;
}

.xsmall {
    font-size: 11px;
}

.xxsmall {
    font-size: 10px;
}
</style>
