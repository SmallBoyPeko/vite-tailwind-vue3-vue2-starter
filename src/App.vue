<template>
  <div id="app">
    <div class="text-center text-3xl font-bold dark:text-white">Vue2 写法</div>
    <div class="text-center dark:text-white mt-4">{{name}}, {{key}}</div>
    <main>
      <RouterView />
    </main>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',
  data() {
    return {
      key: '我是测试key',
    }
  },
  computed: {
    name() {
      return '我是测试name'
    },
  },
  methods: {
    log() {
      console.log(1)
    },
  },
  mounted() {
    this.log()
  },
})
</script>
