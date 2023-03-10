<script setup>
import { ref } from 'vue'

const msg=ref("和声音乐后台")
const count = ref(0)
const hi=()=>{
  msg.value = "已请求"
}
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="button-container">
    <button type="button" @click="count++">点击次数{{ count }}</button>
      <button type="button" @click="hi">请求接口{{ count }}</button>
  </div>


</template>



<style scoped>
.read-the-docs {
  color: #888;
}

.button-container{
  width: 50%;
  display: flex;
  flex-direction: row;
}
</style>
