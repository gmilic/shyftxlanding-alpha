<template>
    <v-container
        fluid
        class="ma-0 pa-0"
    >
        <div class="wrapper">
            <div class="sliding-bg">
            <div ref="draggableContainer" id="draggable-container" @mousedown="dragMouseDown" :style="{ 'left': handPosition }">
                <img name="phone" class="phone" src="/img/ShyftX_hand.png" alt="phone" />
                <h4 v-if="showDragMe">Drag me!</h4>
            </div>
            <transition name="fade">
                <div v-show="showChair" class="chairData overlayData" >
                <div class="overlayDataTitle">Chair</div>
                <div class="overlayDataInfo">
                    <p>Total weight: 55.0</p>
                    <p>Dimensions: 32” x 40” x 30</p>
                    <p>Units: 1</p>
                </div>
                </div>
            </transition>
            <transition name="fade">
                <div v-if="showTV" class="tvData overlayData">
                <div class="overlayDataTitle">TV</div>
                <div class="overlayDataInfo">
                    <p>Total weight: 55.0</p>
                    <p>Dimensions: 32” x 40” x 30</p>
                    <p>Units: 1</p>
                </div>
                </div>
            </transition>
            <transition name="fade">
                <div v-if="showSofa" class="sofaData overlayData">
                <div class="overlayDataTitle">Sofa</div>
                <div class="overlayDataInfo">
                    <p>Total weight: 55.0</p>
                    <p>Dimensions: 32” x 40” x 30</p>
                    <p>Units: 1</p>
                </div>
                </div>
            </transition>
            </div>
        </div>
    </v-container>
</template>

<script>
export default {
  name: 'SurveyDemo',
  data: function () {
    return {
      positionX: undefined,
      movementX: 0,
      showDragMe: true,
      showChair: false,
      showTV: false,
      showSofa: false,
      handPosition: '15vw',
      windowsWidth: 0
    }
  },
  methods: {
    dragMouseDown: function (event) {
      event.preventDefault()
      this.showDragMe = false;
      // get the mouse cursor position at startup:
      this.positionX = this.convertPXToVW(event.clientX)

      document.onmousemove = this.elementDrag
      document.onmouseup = this.closeDragElement
    },
    elementDrag: function (event) {
      event.preventDefault()
      this.movementX = this.positionX - this.convertPXToVW(event.clientX)
      this.positionX = this.convertPXToVW(event.clientX)
      
      // set the element's new position:
      this.handPosition = (parseInt(this.handPosition) - this.movementX) + 'vw'
      if (parseInt(this.handPosition) > 28 && parseInt(this.handPosition) < 38 ) {
        this.showChair = true
      } else {
        this.showChair = false
      }
      if (parseInt(this.handPosition) > 0 && parseInt(this.handPosition) < 12 ) {
        this.showTV = true
      } else {
        this.showTV = false
      }
      if (parseInt(this.handPosition) > 51 && parseInt(this.handPosition) < 61 ) {
        this.showSofa = true
      } else {
        this.showSofa = false
      }

      
    },
    closeDragElement () {
      document.onmouseup = null;
      document.onmousemove = null;
      // this.showDragMe = true;
      // this.showChair = false;
    },
    convertPXToVW: function(px) {
      return Math.round(px / this.windowsWidth * 100 );
      // if(px > 0) {
      //   return Math.round(px / this.windowsWidth * 100 );
      // } else if (px < 0) {
      //   return -(Math.round(px / this.windowsWidth * 100 ));
      // } else {
      //   return 0
      // }
    }
  },
  computed: {
    // showChairCalc: function() {
    //   if (this.positions.clientX > 970 ) {
    //     return this.showChair = true
    //   } else {
    //     return this.showChair = false
    //   }
    // }
  },
  mounted() {
      this.windowsWidth =  document.documentElement.clientWidth
  }
}
</script>

<style scoped>
  .wrapper {
    overflow: hidden;
  }
  .sliding-bg {
    position: relative;
    background: url('/img/ShyftX_room.jpg') no-repeat left center;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    width: 100vw;
    max-width:100%;
    height: 30vw;
    animation: slide 60s linear infinite;
  }
  .phone {
    width: 67vw;
    vertical-align: bottom;
  }
  #draggable-container {
    position: absolute;
    bottom: 0;
    width: 67vw;
    z-index: 9;
  }
  h4 {
    color: #eee;
    text-shadow: 2px 2px 6px #000;
    font-size: 2em;
    position: absolute;
    top: 39%;
    left: 16%;
    font-family: sans-serif;
  }
  .chairData {
    position: absolute;
    top: 12vw;
    left: 46vw;
    
  }
  .tvData {
    position: absolute;
    top: 10vw;
    left: 16vw;
  }
  .sofaData {
    position: absolute;
    top: 11vw;
    left: 65vw;
  }
  .overlayData {
    transition: all 0.3s ease-in-out;
  }
  .overlayDataTitle {
    width: 63px;
    height: 23px;
    background: #4C82BF;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.35);
    border-radius: 10px 10px 0 0;
    color: #fff;
    font-size: 14px;
    padding: 2px 0 0 6px;
  }
  .overlayDataInfo {
    width: 168px;
    height: 64px;
    background: #FFFFFF;
    border-radius: 0 10px 10px 10px;
    font-size: 12px;
    line-height: 127.5%;
    padding: 10px 6px 6px 6px;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.4);
  }
  .overlayDataInfo p {
    font-size: 12px;
    line-height: 1.2;
    margin: 0;
    color: #000;
  }
  .fade-enter-active, .fade-leave-active {
    transition: opacity .3s;
  }
  .fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
    opacity: 0;
  }
</style>