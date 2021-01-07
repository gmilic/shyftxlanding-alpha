<template>
  <section>
    <AppHero></AppHero>
    <SecondRow></SecondRow>
    <TabletBids></TabletBids>
    <HowShyftWorks></HowShyftWorks>
    <SurveyDemoTitle></SurveyDemoTitle>
    <SurveyDemoScroll></SurveyDemoScroll>
    <Testimonials></Testimonials>
    <SquareLeft01></SquareLeft01>
    <SquareRight01></SquareRight01>
    <StartBusinessJourney></StartBusinessJourney>
    <SurveyDemoTitle></SurveyDemoTitle>
    <SurveyDemo></SurveyDemo>
    <BlogList></BlogList>
  </section>
</template>

<script>
import AppHero from '~/components/AppHero'
import SecondRow from '~/components/SecondRow'
import TabletBids from '~/components/TabletBids'
import HowShyftWorks from '~/components/HowShyftWorks'
import SquareLeft01 from '~/components/Square-left-01.vue'
import SquareRight01 from '~/components/Square-right-01.vue'
import SurveyDemoTitle from '~/components/SurveyDemoTitle.vue'
import SurveyDemo from '~/components/SurveyDemo.vue'
import SurveyDemoScroll from '~/components/SurveyDemoScroll.vue'
import StartBusinessJourney from '~/components/StartBusinessJourney.vue'
import BlogList from '~/components/BlogList.vue'
import Testimonials from '~/components/Testimonials.vue'


export default {
  components: {
    AppHero,
    SecondRow,
    TabletBids,
    HowShyftWorks,
    SquareLeft01,
    SquareRight01,
    SurveyDemoTitle,
    SurveyDemo,
    StartBusinessJourney,
    BlogList

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