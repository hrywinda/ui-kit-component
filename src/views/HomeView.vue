<template>
  <main>
    <!-- <Button /> -->
    <!-- <div class="container mx-auto bg-gray-200 rounded-xl shadow border p-8 m-10"> -->
    <div>
     <p class="text-3xl text-gray-700 font-bold mb-5">Button</p>
     <div class="grid gap-4 grid-cols-1">
      <jm-button :label="'Custom label'"/>
      <jm-button :label="'Disable Buttton'" :isDisabled="true"/>
      <jm-button :label="'M'" :type="'circle'"/>
      <jm-button :label="'Stroke Button'" :type="'stroke'"/>
    </div>
    <p class="text-3xl text-gray-700 font-bold mb-5">Status</p>
    <div class="grid gap-4 grid-cols-1">
      <jm-status :label="'Custom label'"/>
      <jm-status 
        :label="'Custom label'" 
        :type="'secondary'" 
        :bgColor="`bg-[#DDD6ED]`"/>
    </div>
  </div>
  </main>
</template>

<script>
import Button from '../components/Button.vue'
import Status from '../components/Status.vue'

export default {
  name: 'home',
  components: {
    'jm-button': Button,
    'jm-status': Status
  }
}

</script>