<template>
  <div id="app" v-hotkey="keymap">
    <SpiritBoard/>
  </div>
</template>

<script>
import SpiritBoard from "./components/SpiritBoard.vue";

export default {
  name: 'App',
  components: {
    SpiritBoard
  },
  methods: {
    forest1() {
      document.body.classList='forest1'
    },
    forest2() {
      document.body.classList='forest2'
    },
    forest3() {
      document.body.classList='forest3'
    },
    forest4() {
      document.body.classList='forest4'
    },
    forest5() {
      document.body.classList='forest5'
    }
  },
  computed: {
    keymap() {
      return {
        // card types
        'ctrl+1': this.forest1,
        'ctrl+2': this.forest2,
        'ctrl+3': this.forest3,
        'ctrl+4': this.forest4,
        'ctrl+5': this.forest5
      }
    }
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
