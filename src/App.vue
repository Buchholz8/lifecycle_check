<template>
  <div id="app">
    <life-cycle-example></life-cycle-example>
    <show-info></show-info>
    <template-fun></template-fun>
  </div>
</template>

<script>
import LifeCycleExample from '@/components/LifecycleExample.vue'
import ShowInfo from '@/components/ShowInfo.vue'
import TemplateFun from '@/components/TemplateFun.vue'
export default {
  name: 'App',
  components: {
    LifeCycleExample,
    ShowInfo,
    TemplateFun,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
