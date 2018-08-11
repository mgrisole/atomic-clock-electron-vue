<template lang="pug">
  v-flex(justify-content-center align-content-center)
    | {{timer}}
</template>

<script>
import moment from 'moment'

export default {
  name: 'ModuleTimer',
  data () {
    return {
      timer: ''
    }
  },
  methods: {
    update () {
      setInterval(() => {
        // this.timer = moment().format('LTS')
      }, 1000)
    }
  },
  created () {
    moment.locale('fr')
    this.timer = moment().format('LTS')
  },
  mounted () {
    this.update()
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">

</style>
