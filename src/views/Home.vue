<template lang="pug">
  v-container(fluid fill-height)
    v-slide-y-transition(mode="out-in")
      v-layout(align-center fill-height column justify-center )
        ModuleTimer
        ModuleTimer 
</template>

<script>
import ModuleTimer from './modules/Timer'

export default {
  name: 'HomeView',
  components: {
    ModuleTimer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
</style>
