<template>
    <button @click="onClick" :class="[bgColor, textColor, isDisabled ? 'disabled' : '', `btn-${type}`]">
      {{label}}
    </button>
</template>

<script>
export default {
  name: 'jm-button',
  components: {

  },
  props: {
    label: {
      required: false
    },
    color:{
      required: false
    },
    isDisabled:{
      type:Boolean,
      required: false,
      default:false
    },
    textColor:{
      required: false,
      default: ''
    }, 
    bgColor:{
      required: false,
      default: ''
    },
    type:{
      //filled, stroke, circle, no border
      required: false,
      default: "filled"
    }
  },
  methods:{
    getType(type){
      return `btn-type`
    }
  }
}
</script>

<style scoped>
@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
