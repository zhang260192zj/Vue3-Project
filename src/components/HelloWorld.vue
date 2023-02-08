<template>
 <h1>{{a}}</h1>
 <button @click="add">Add</button>
</template>
<script>
import { defineComponent ,reactive,ref} from 'vue'

export default defineComponent({
  setup () {
    let a = ref(1)
    const obj = {
      a:1
    }
    let b =reactive(obj)
    console.log(obj,b)
    const add =()=>{

    }
    return {
      a,
      obj,
      add,
    }
  }
})
</script>

<style scoped>

</style>
