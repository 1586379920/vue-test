<template>
  <h1>{{data.name}}</h1>
  <button @click="changeNumber">an</button>
</template>

<script>
import { reactive } from "vue"

export default {
  name: 'App',
  setup(){
    let data=reactive({
      name:'jungle'
    })
    function changeNumber(){
      console.log(data)
    }
    return {
      data,
      changeNumber
    }
  }
}
</script>

