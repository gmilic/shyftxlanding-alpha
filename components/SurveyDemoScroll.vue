<template>
<div class="demoScroll mb-16" ref="demoScroll">
  <div class="animWrapper">
    <div class="phoneContainer" ref="phoneContainerStyles">
      <img class="phone" src="img/ShyftX_hand.png" alt="phone" />
      <!-- <h4 class="pleaseScroll" >Please scroll</h4> -->
    </div>
    <transition name="fade">
      <div class="chairData overlayData" >
        <div class="overlayDataTitle">Chair</div>
        <div class="overlayDataInfo">
          <p>Total weight: 55.0</p>
          <p>Dimensions: 32” x 40” x 30</p>
          <p>Units: 1</p>
        </div>
      </div>
    </transition>
    <transition name="fade">
      <div class="tvData overlayData">
        <div class="overlayDataTitle">TV</div>
        <div class="overlayDataInfo">
          <p>Total weight: 55.0</p>
          <p>Dimensions: 32” x 40” x 30</p>
          <p>Units: 1</p>
        </div>
      </div>
    </transition>
    <transition name="fade">
      <div class="sofaData overlayData">
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
</template>

<script>
  import { gsap } from "gsap";
  import { ScrollTrigger } from "gsap/ScrollTrigger";

export default {
  name: 'SurveyDemoScroll',
  data: function () {
    return {
      animPosition: 0,
      animHeight: 0
    }
  },  
  methods: {
    calcPosOfBox () {
      // this.animPosition = this.$refs['demoScroll'].getBoundingClientRect().top;
      this.animPosition = this.offset(this.$refs['demoScroll']);
      // this.animHeight = this.animPosition + this.$refs['demoScroll'].offsetHeight;
      console.log(this.animPosition.top);
      // console.log(this.animHeight);
    },
    offset(el) {
      var rect = el.getBoundingClientRect(),
      scrollLeft = window.pageXOffset || document.documentElement.scrollLeft,
      scrollTop = window.pageYOffset || document.documentElement.scrollTop;
      return { top: rect.top + scrollTop, left: rect.left + scrollLeft }
    },
    onScroll() {
      let tempAnimPosition = this.offset(this.$refs['demoScroll']);
      if (this.animPosition.top != tempAnimPosition.top) {
        this.animPosition = this.offset(this.$refs['demoScroll']);
      }
    }
  },
  computed: {

  },
  watch: {
    animPosition() {
      console.log('pos changed');
      ScrollTrigger.refresh(true);
    }
  },
  mounted() {
      this.animHeight = this.animPosition + this.$refs['demoScroll'].offsetHeight;
      window.addEventListener('scroll', this.onScroll);

      gsap.registerPlugin(ScrollTrigger);
      
      let tl = gsap.timeline({
        scrollTrigger: {
          trigger: ".demoScroll",
          scrub: true,
          pin: ".animWrapper",
          start: "top 64px",
          end: "+=" + (this.animHeight * 2),
          // end: this.animHeight,
          // end: "bottom bottom",
          // toggleActions: "restart reverse restart reverse",
          // snap: {
          //   snapTo: "labels", // snap to the closest label in the timeline
          //   duration: {min: 0.2, max: 3}, // the snap animation should be at least 0.2 seconds, but no more than 3 seconds (determined by velocity)
          //   delay: 0.2, // wait 0.2 seconds from the last scroll event before doing the snapping
          //   ease: "power1.inOut" // the ease of the snap animation ("power3" by default)
          // },
          // markers: true,
        }
      })

      tl
        .fromTo('.tvData', {
          opacity: 1
        },
        {
          opacity: 0,
          ease: "power4.in"
        })
        .to('.phoneContainer', {
          x: "33vw", 
        })
        .fromTo('.chairData', {
          opacity: 0
        },
        {
          opacity: 1,
          ease: "power4.out"
        })
        .fromTo('.chairData', {
          opacity: 1
        },
        {
          opacity: 0,
          ease: "power4.in"
        })
        .to('.phoneContainer', {
          x: "56vw", 
        })
        .fromTo('.sofaData', {
          opacity: 0
        },
        {
          opacity: 1,
          ease: "power4.out"
        })
        .fromTo('.sofaData', {
          opacity: 1
        },
        {
          opacity: 0,
          ease: "power4.in"
        })

  },
  beforeDestroyed() {
    let triggers = ScrollTrigger.getAll();
      triggers.forEach( trigger => {			
        trigger.kill();
      });
  }


}
</script>

<style scoped>
  .animWrapper {
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
  .demoScroll {
    position:relative;
  }
  .phoneContainer {
    position: absolute;
    bottom: 0;
    z-index: 9;
    /* left: 3vw; */
  }
   .phone {
    width: 67vw;
    vertical-align: bottom;
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
  .showChairWrapp {
    color: #eee;
    text-shadow: 2px 2px 6px #000;
    font-size: 2em;
    position: absolute;
    top: 39%;
    left: 16%;
    font-family: sans-serif;
  }
  .phoneAnimImg {
    width: 30vw;
  }
    .chairData {
    position: absolute;
    top: 12vw;
    left: 42vw;
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
    transition: all 0.2s ease-in-out;
    opacity: 0
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