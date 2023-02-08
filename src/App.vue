<template>
  <component :is="hello"></component>
</template>

<script>
import { defineComponent} from 'vue'
import HelloWorld from './components/HelloWorld.vue';
export default defineComponent({
  setup () {
    return {
      hello:HelloWorld
    }
  }
})
</script>

<style scoped>

</style>
