<template>
 <h1>{{num.b.c}}</h1>
 <button @click="add">Add</button>
</template>
<script>
import { defineComponent ,reactive,ref} from 'vue'

export default defineComponent({
  setup () {
    const data =reactive({
      num:{
        a:1,
        b:{
          c:1
        }
      }
    })
    const add=()=>{
      data.num.b.c++
    }
    return {
      ...data,
      add
    }
  }
})
</script>

<style scoped>

</style>
