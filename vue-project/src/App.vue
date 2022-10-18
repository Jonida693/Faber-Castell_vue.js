<script>
import Header from "./components/Header.vue";
import "./assets/grid.css";
import navMenu from "./components/navMenu.vue";
import SliderCarousel from "./components/SliderCarousel.vue";
import MapComponent from "./components/MapComponent.vue";
import OnlySlider2 from "./components/OnlySlider2.vue";
import SocialMedia from "./components/SocialMedia.vue";
import Payments from "./components/Payments.vue";
import Footer from "./components/Footer.vue"

export default {
  data: () => {
    return {};
  },
  methods: {},
  components: {
    Header,
    navMenu,

    SliderCarousel,
    MapComponent,
    OnlySlider2,
    SocialMedia,
    Payments,
    Footer,
   
  },
};
</script>
<template>
  <Header />
  <navMenu />
  <SliderCarousel />
  <MapComponent />
  <OnlySlider2/>
  <SocialMedia/>
  <Payments/>
  <Footer/>

</template>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  position: relative;
  color: black;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  line-height: 26px;
  min-height: 100%;
  margin: 0 auto;
  /* max-width: 2600px; */
  background-color: #f6f6f0;
  /* min-width: 1280px; */
}
a {
  text-decoration: none;
  color: unset;
}
a:hover {
  cursor: pointer;
  color: #05301a;
}
span.wrapper-stars {
  color: orange;
  font-size: 20px;
  line-height: 0;
}

button.btn {
  border-radius: 3px;
  background: rgb(198, 188, 151);
  border: none;
  color: #ffffff;
  cursor: pointer;
  display: inline-block;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 14px;
  letter-spacing: 0.035em;
  line-height: 21px;
  margin-top: 26px;
  padding: 10px 14px 10px;
  opacity: 1; 
     margin-bottom: 20px;

}
</style>
