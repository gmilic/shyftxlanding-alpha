<template>
  <section>
    <AppHero />
    <SecondRow />
    <TabletBids />
    <HowShyftWorks />
    <SurveyDemoTitle />
    <SurveyDemoScroll />
    <GrowWithShyftx />
    <Testimonials />
    <BlogList />
    <IndustryPress />
    <GetInTouch />
  </section>
</template>

<script>
import AppHero from '~/components/AppHero'
import SecondRow from '~/components/SecondRow'
import TabletBids from '~/components/TabletBids'
import HowShyftWorks from '~/components/HowShyftWorks'
import GrowWithShyftx from '~/components/GrowWithShyftx'
import SurveyDemoTitle from '~/components/SurveyDemoTitle.vue'
import SurveyDemoScroll from '~/components/SurveyDemoScroll.vue'
import BlogList from '~/components/BlogList.vue'
import IndustryPress from '~/components/IndustryPress.vue'
import Testimonials from '~/components/Testimonials.vue'
import GetInTouch from '~/components/GetInTouch.vue'


export default {
  components: {
    AppHero,
    SecondRow,
    TabletBids,
    HowShyftWorks,
    GrowWithShyftx,
    SurveyDemoTitle,
    SurveyDemoScroll,
    BlogList,
    IndustryPress,
    GetInTouch

  }
}
</script>

<style>
.mainButtonSignUp {
  background-color: #EB344A;
  color: #fff;
  box-shadow:0px 7px 67px rgba(235, 52, 74, 0.25);
  padding: 22px 40px;
  border-radius: 10px;
  text-align: center;
  width: fit-content; 
  font-weight: 700;
  font-size: 1.3em;
  margin: 24px 0;
}
</style>