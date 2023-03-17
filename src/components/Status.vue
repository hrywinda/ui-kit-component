<template>
  <div :class="['jm-status', textColor, bgColor, 
    type == 'primary' ? 'primary': 'secondary']">
    {{ label }}
  </div>
</template>

<script>
export default {
  name: 'jm-status-label',
  components: {

  },
  props: {
    label: {
      required: false
    },
    textColor:{
      required: false,
      default: 'text-[#006664]'
    }, 
    bgColor:{
      //add arbitrary hex color value
      required: false,
      default: 'bg-[#CCE0E0]'
    },
    type:{
      //primary, secondary
      required: false,
      default: "primary"
    },
    // icon:{
        
    // }
  }
}
</script>

<style scoped>
</style>
