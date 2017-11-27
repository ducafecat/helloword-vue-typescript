<template>
  <div>
    <input v-model="msg">
    <p>msg: {{ msg }}</p>
    <button @click="handelHello">hello</button>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue'
  import Component from 'vue-class-component'

  @Component
  export default class App extends Vue {
    // 初始化数据
    msg: string = 'hello word'

    mounted () {
    }

    // 方法
    handelHello () {
      this.msg = 'haha~~~ hello word!'
    }
  }
</script>