<template>
  <section class="carousel-full">
    <Carousel :infinite="true">
      <Slide v-for="slide in 4" :key="slide">
        <div class="carusel-images">
          <div class="slide-carusel">
            <div class="background-img">
              <img
                src="https://www.faber-castell.de/-/media/Faber-Castell-new/did-you-know/did-you-know-hexagonal.ashx?la=de-DE&h=400&w=1280&mw=2600&hash=2727FE077DEE4285BA00B61E57651A83A88DD400"
              />
              <div class="wrap">
                <div class="body-slider">
                  <div class="title">Wussten Sie schon?</div>
                  <div class="desc">
                    Faber-Castell benutzt ausschließlich Holz aus nachhaltig
                    bewirtschafteten Forsten für die eigene Stifteproduktion.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>
  </section>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Navigation, Pagination, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

export default defineComponent({
  name: "Basic",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data: () => {
    return {};
  },
});
</script>

<style lang="scss">
.carousel-full {
  max-width: 1903px;
  .carousel {
    height: 500px;
    margin: 0 auto;
    width: 100vw;

    .carousel__viewport {
      overflow: unset;
      height: 100%;
    }
  }
  .carousel__item {
    position: absolute;
  }

  .carousel__slide {
    opacity: 0;
    transition: opacity 0.4s;
  }

  .carousel__track {
    width: 100%;
  }

  .carousel__slide.carousel__slide--active.carousel__slide--visible {
    opacity: 1;
    transition: opacity 0.4s;
  }

  .carousel__pagination-button {
    cursor: pointer;
    background-color: #f6f6f0;
    width: 10px;
    height: 10px;
    display: block;
    cursor: pointer;
    text-indent: -9999px;
    box-shadow: inset 0.5px 0.866px 3px 0 rgb(0 0 0 / 40%);
  }
  .carousel__pagination {
    display: flex;
    justify-content: center;
    list-style: none;
    background-color: unset;
    position: absolute;
    left: 40%;
    top: 105%;
  }

  .carousel__pagination-button--active {
    background-color: #004b37;
  }

  // .carousel__prev,
  // .carousel__next {
  //   box-sizing: content-box;
  //   border: 5px solid white;
  // }

  .carousel__next {
background-color: transparent;
    position: absolute;
    top: 60%;
    height: 85px;
    margin-top: 0;
    width: 85px;
        right: 50px;
  
  
  }

  .carousel__prev {
 background-color: transparent;
    position: absolute;
    top: 60%;
    height: 85px;
    margin-top: 0;
    width: 85px;
    left: 15px;
  }

  .carousel__prev::before {
    content: "";
    border-left: 1px solid
      var(--PaginationBulletsPrimaryColor, var(--BaseFontColor));
    border-top: 1px solid
      var(--PaginationBulletsPrimaryColor, var(--BaseFontColor));
    display: block;
    height: 24px;
    position: relative;
    width: 24px;
    left: -6px;
    transform: rotate(135deg);
  }

  .carousel__next::before {
    content: "";
    border-left: 1px solid
      var(--PaginationBulletsPrimaryColor, var(--BaseFontColor));
    border-top: 1px solid
      var(--PaginationBulletsPrimaryColor, var(--BaseFontColor));
    display: block;
    height: 24px;
    position: relative;
    width: 24px;
    left: -6px;
    transform: rotate(135deg);
  }

  .carousel_icon {
    font-size: 60px;
    fill: currentColor;
  }
  .carusel-images {
    width: 100%;
  }
  .background-img {
    position: relative;
    img {
      width: 100%;
    }
    .wrap {
      position: absolute;
      top: 40%;
      color: white;
      left: 15%;
      line-height: 62px;
      font-size: 23px;
      font-style: italic;
      max-height: 30px;
      text-align: center;
    }
  }
}
</style>
