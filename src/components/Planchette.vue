<template>
  <div id="planchette" :class="[positionClass]" v-hotkey="keymap">
    <img src="../assets/planchette.png">
  </div>
</template>

<script>
export default {
  name: "Planchette",
  data() {
    return {
      positionClass: ''
    }
  },
  methods: {
    // center and card types
    posEye() {
      this.positionClass = ""
    },
    posCrown() {
      this.positionClass = "crown"
    },
    posCoin() {
      this.positionClass = "coin"
    },
    posSword() {
      this.positionClass = "sword"
    },
    posStar() {
      this.positionClass = "star"
    },
    posGlyph() {
      this.positionClass = "glyph"
    },

    // Yes and No
    posYes() {
      this.positionClass = "yes"
    },
    posNo() {
      this.positionClass = "no"
    },

    // Numbers
    posZero() {
      this.positionClass = "zero"
    },
    posOne() {
      this.positionClass = "one"
    },
    posTwo() {
      this.positionClass = "two"
    },
    posThree() {
      this.positionClass = "three"
    },
    posFour() {
      this.positionClass = "four"
    },
    posFive() {
      this.positionClass = "five"
    },
    posSix() {
      this.positionClass = "six"
    },
    posSeven() {
      this.positionClass = "seven"
    },
    posEight() {
      this.positionClass = "eight"
    },
    posNine() {
      this.positionClass = "nine"
    },

    // Letters
    posA() {
      this.positionClass = "letterA"
    },
    posB() {
      this.positionClass = "letterB"
    },
    posC() {
      this.positionClass = "letterC"
    },
    posD() {
      this.positionClass = "letterD"
    },
    posE() {
      this.positionClass = "letterE"
    },
    posF() {
      this.positionClass = "letterF"
    },
    posG() {
      this.positionClass = "letterG"
    },
    posH() {
      this.positionClass = "letterH"
    },
    posI() {
      this.positionClass = "letterI"
    },
    posJ() {
      this.positionClass = "letterJ"
    },
    posK() {
      this.positionClass = "letterK"
    },
    posL() {
      this.positionClass = "letterL"
    },
    posM() {
      this.positionClass = "letterM"
    },
    posN() {
      this.positionClass = "letterN"
    },
    posO() {
      this.positionClass = "letterO"
    },
    posP() {
      this.positionClass = "letterP"
    },
    posQ() {
      this.positionClass = "letterQ"
    },
    posR() {
      this.positionClass = "letterR"
    },
    posS() {
      this.positionClass = "letterS"
    },
    posT() {
      this.positionClass = "letterT"
    },
    posU() {
      this.positionClass = "letterU"
    },
    posV() {
      this.positionClass = "letterV"
    },
    posW() {
      this.positionClass = "letterW"
    },
    posX() {
      this.positionClass = "letterX"
    },
    posY() {
      this.positionClass = "letterY"
    },
    posZ() {
      this.positionClass = "letterZ"
    },

    // Greetings
    posGreetings() {
      this.positionClass = "greetings"
    },
    posFarewell() {
      this.positionClass = "farewell"
    }
  },
  computed: {
    keymap() {
      return {
        // card types
        'shift+c': this.posCrown,
        'ctrl+c': this.posCoin,
        'shift+e': this.posEye,
        'shift+g': this.posGlyph,
        'shift+s': this.posSword,
        'ctrl+s': this.posStar,

        // yes and no
        'shift+y': this.posYes,
        'shift+n': this.posNo,

        // numbers
        '0': this.posZero,
        '1': this.posOne,
        '2': this.posTwo,
        '3': this.posThree,
        '4': this.posFour,
        '5': this.posFive,
        '6': this.posSix,
        '7': this.posSeven,
        '8': this.posEight,
        '9': this.posNine,

        //letters
        'a': this.posA,
        'b': this.posB,
        'c': this.posC,
        'd': this.posD,
        'e': this.posE,
        'f': this.posF,
        'g': this.posG,
        'h': this.posH,
        'i': this.posI,
        'j': this.posJ,
        'k': this.posK,
        'l': this.posL,
        'm': this.posM,
        'n': this.posN,
        'o': this.posO,
        'p': this.posP,
        'q': this.posQ,
        'r': this.posR,
        's': this.posS,
        't': this.posT,
        'u': this.posU,
        'v': this.posV,
        'w': this.posW,
        'x': this.posX,
        'y': this.posY,
        'z': this.posZ,


        // greetings
        'ctrl+g': this.posGreetings,
        'ctrl+f': this.posFarewell
      }
    }
  }
}
</script>

<style scoped>
#planchette {
  position: absolute;
  top: 356px;
  left: 312px;
  -webkit-transition: 4s all ease;
  -moz-transition: 4s all ease;
  -ms-transition: 4s all ease;
  transition: 4s all ease;
}

#planchette img {
  animation: float 3700ms ease-in-out infinite;
  height: 184px;
}

/* card types */
.crown {
  transform: translateY(-99px);
}

.coin {
  transform: translate(96px, -5px) rotate(12deg);
}

.glyph {
  transform: translate(64px, -73px) rotate(6deg);
}

.sword {
  transform: translate(-91px, -5px) rotate(-16deg);
}

.star {
  transform: translate(-57px, -74px) rotate(-21deg);
}

/* yes and no */
.yes {
  transform: translate(-146px, 54px) rotate(27deg);
}

.no {
  transform: translate(146px, 54px) rotate(-27deg);
}

/* numbers */

.zero {
  transform: translate(-142px, -105px) rotate(20deg);
}
.one {
  transform: translate(-112px, -130px) rotate(12deg);
}
.two {
  transform: translate(-82px, -148px) rotate(15deg);
}
.three {
  transform: translate(-52px, -154px) rotate(18deg);
}
.four {
  transform: translate(-18px, -160px) rotate(8deg);
}
.five {
  transform: translate(22px, -164px) rotate(-10deg);
}
.six {
  transform: translate(52px, -154px) rotate(-18deg);
}
.seven {
  transform: translate(82px, -148px) rotate(-12deg);
}
.eight {
  transform: translate(116px, -135px) rotate(-15deg);
}
.nine {
  transform: translate(142px, -105px) rotate(-26deg);
}

/* letters */
.letterA {
  transform: translate(-223px, -104px) rotate(120deg);
}

.letterB {
  transform: translate(-188px, -160px) rotate(132deg);
}

.letterC {
  transform: translate(-158px, -195px) rotate(140deg);
}

.letterD {
  transform: translate(-123px, -220px) rotate(148deg);
}

.letterE {
  transform: translate(-82px, -245px) rotate(156deg);
}

.letterF {
  transform: translate(-42px, -265px) rotate(164deg);
}

.letterG {
  transform: translate(8px, -260px) rotate(176deg);
}

.letterH {
  transform: translate(58px, -250px) rotate(188deg);
}

.letterI {
  transform: translate(98px, -237px) rotate(203deg);
}

.letterJ {
  transform: translate(131px, -212px) rotate(213deg);
}

.letterK {
  transform: translate(163px, -191px) rotate(226deg);
}

.letterL {
  transform: translate(204px, -160px) rotate(236deg);
}

.letterM {
  transform: translate(218px, -108px) rotate(246deg);
}

.letterN {
  transform: translate(-223px, 34px) rotate(74deg);
}

.letterO {
  transform: translate(-208px, 94px) rotate(61deg);
}

.letterP {
  transform: translate(-176px, 134px) rotate(48deg);
}

.letterQ {
  transform: translate(-140px, 172px) rotate(33deg);
}

.letterR {
  transform: translate(-93px, 202px) rotate(17deg);
}

.letterS {
  transform: translate(-45px, 212px) rotate(9deg);
}

.letterT {
  transform: translate(-2px, 220px) rotate(359deg);
}

.letterU {
  transform: translate(53px, 212px) rotate(350deg);
}

.letterV {
  transform: translate(102px, 198px) rotate(338deg);
}

.letterW {
  transform: translate(151px, 167px) rotate(323deg);
}

.letterX {
  transform: translate(192px, 123px) rotate(309deg);
}

.letterY {
  transform: translate(224px, 78px) rotate(292deg);
}

.letterZ {
  transform: translate(238px, 25px) rotate(284deg);
}

/* greetings */
.greetings {
  transform: translate(-140px, 140px) rotate(45deg);
}

.farewell {
  transform: translate(155px, 85px) rotate(-115deg);
}

@keyframes float {
  0% {
    transform: translatey(0px) scale(1) rotate(0deg);
  }
  50% {
    transform: translatey(-5px) scale(1.05) rotate(3deg);
  }
  100% {
    transform: translatey(0px) scale(1) rotate(0deg);
  }
}

</style>