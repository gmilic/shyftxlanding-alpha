<template>
  <section>
    <AppHero></AppHero>
    <ThreeCTA></ThreeCTA>
    <Text-01></Text-01>
    <Laptop-01></Laptop-01>
    <Square-left-01></Square-left-01>
    <Square-right-01></Square-right-01>
    <SurveyDemoTitle></SurveyDemoTitle>
    <SurveyDemo></SurveyDemo>
    <StartBusinessJourney></StartBusinessJourney>
    <BlogList></BlogList>
  </section>
</template>

<script>
import AppHero from '~/components/AppHero'
import ThreeCTA from '~/components/ThreeCTA'
import Text01 from '~/components/Text01'
import Laptop01 from '~/components/Laptop01'
import SquareLeft01 from '~/components/Square-left-01.vue'
import SquareRight01 from '~/components/Square-right-01.vue'
import SurveyDemoTitle from '~/components/SurveyDemoTitle.vue'
import SurveyDemo from '~/components/SurveyDemo.vue'
import StartBusinessJourney from '~/components/StartBusinessJourney.vue'
import BlogList from '~/components/BlogList.vue'

export default {
  components: {
    AppHero,
    ThreeCTA,
    Text01,
    Laptop01,
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

</style>