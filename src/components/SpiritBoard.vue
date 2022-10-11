<template>
  <div id="outer">
    <img id="spiritboard" src="../assets/spiritboard.png">
    <Planchette/>
  </div>
</template>

<script>
import Planchette from "@/components/Planchette";
export default {
  name: "SpiritBoard",
  components: {Planchette}
}
</script>

<style scoped>
div#outer {
  margin: 0 auto;
  height: 880px;
  width: 768px;
  position: relative;
}
img#spiritboard {
  height: 96%;
  animation: float 7s ease-in-out infinite;
}

@keyframes float {
  0% {
    transform: translatey(0px) scale(1) rotate(0deg);
  }
  50% {
    transform: translatey(-2px) scale(1.01) rotate(-.25deg);
  }
  100% {
    transform: translatey(0px) scale(1) rotate(0deg);
  }
}
</style>