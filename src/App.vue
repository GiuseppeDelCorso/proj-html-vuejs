<script>
import AppHeader from './components/AppHeader.vue'
import AppMain1 from './components/AppMain1.vue'
import AppMain2 from './components/AppMain2.vue'
import CategoriesMain from './components/CategoriesMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain1,
    AppMain2,
    CategoriesMain,
    AppFooter,

  },
  data() {
    return {
      categories: [
        {
          type: "All categories"
        },
        {
          type: "Buisness"
        },
        {
          type: "Desing"
        },
        {
          type: "Development"
        },
        {
          type: "IT & Software"
        },
        {
          type: "Lifestyle"
        },
        {
          type: "Marketing"
        },
        {
          type: "Office Productivity"
        },

      ],
      cardInfo: [
        {
          img: "186792_41e4_4-272x161",
          typeCourses: "Development",
          infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
          price: "Free",
          star: "20"
        },
        {
          img: "246154_d8b0_3-272x161",
          typeCourses: "Desing",
          infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
          price: "100$",
          star: 20
        },
        {
          img: "1253188_58f7_2-272x161",
          typeCourses: "Development",
          infoCourses: "Web Design for Beginners: Real World Coding in HTML & CSS",
          price: "65$",
          star: 20
        },
        {
          img: "1414956_d944_15-272x161",
          typeCourses: "Desing",
          infoCourses: "Digitally Painting Light and Color: Amateur to Master",
          price: "70$",
          star: 20
        },
        {
          img: "1561458_7f3b-272x161",
          typeCourses: "Art And Crafts",
          infoCourses: "Become an Arabic Calligraphy Artist from Scratch",
          price: "199$",
          star: 20
        },
        {
          img: "1776542_30b1-272x161",
          typeCourses: "Google",
          infoCourses: "Google Searching Ninja!",
          price: "45$",
          star: 20
        },
        {
          img: "838056_611a_3-272x161",
          typeCourses: "Development",
          infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
          price: "Free",
          star: "20"
        },
        {
          img: "895786_7b4b_2-272x161",
          typeCourses: "Desing",
          infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
          price: "100$",
          star: 20
        },
        {
          img: "919872_ed54_6-272x161",
          typeCourses: "Development",
          infoCourses: "Web Design for Beginners: Real World Coding in HTML & CSS",
          price: "65$",
          star: 20
        },
        {
          img: "949316_2a64_11-272x161",
          typeCourses: "Desing",
          infoCourses: "Digitally Painting Light and Color: Amateur to Master",
          price: "70$",
          star: 20
        },
        {
          img: "951684_9c1a_2-272x161",
          typeCourses: "Art And Crafts",
          infoCourses: "Become an Arabic Calligraphy Artist from Scratch",
          price: "199$",
          star: 20
        },
        {
          img: "1208228_d61c_4-272x161",
          typeCourses: "Google",
          infoCourses: "Google Searching Ninja! go go go",
          price: "45$",
          star: 20
        },

      ],
    }
  }

}
</script>

<template>
  <section>
    <AppHeader />
  </section>
  <section>
    <AppMain1 />
  </section>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="styleTitleMain2">Recent courses</h1>
        </div>
      </div>
    </div>
    <div class="container d-flex mb-4">
      <CategoriesMain v-for="data in this.categories" :linkcategories="data" />
    </div>
  </section>
  <section>
    <div class="container d-flex justify-content-between flex-wrap my-5">
      <AppMain2 v-for="cards in this.cardInfo" :linksCards="cards" />
    </div>
  </section>
  <section>
    <AppFooter />
  </section>
</template>

<style scoped>
.styleTitleMain2 {
  font-weight: bold;
  text-align: center;
  padding-bottom: 30px;
}
</style>
