<template>
  <Carousel :infinite="true">
    <Slide v-for="slide in 2" :key="slide">
      <div class="carousel__item">
        <div>
          <div class="slider">
            <div class="header">
              <img
                src="https://www.faber-castell.de/-/media/Faber-Castell-new/special-pages/creative-moments/stage-teaser-creative-moments.ashx?la=de-DE&h=400&w=948&mw=948&hash=1A8CEDC18A2A7BCEC8D8402793A5C5323A495621"
                alt=""
              />
            </div>
            <div class="body">
              <div class="title">Nimm Dir eine analoge Pause</div>
              <div class="description">
                Füller, Kugelschreiber und Druckbleistift in den drei sanften,
                gedämpften Farben Coconut Milk, Rose Shadows und Dapple Gray –
                perfekt für die vielen Zwischentöne in Deinem Alltag.
              </div>
              <a href=""> Mehr erfahren </a>
            </div>
          </div>
        </div>
      </div>
      <div>
        <div class="slider">
          <div class="header">
            <img
              src="https://www.faber-castell.de/-/media/Faber-Castell-new/special-pages/write-future/stage-teaser-write-your-own-future.ashx?la=de-DE&h=400&w=948&mw=948&hash=DA904F69A4726CDBB271515C1E8C50B610804478"
              alt=""
            />
          </div>
          <div class="body">
            <div class="title">Nimm Dir eine analoge Pause</div>
            <div class="description">
              Füller, Kugelschreiber und Druckbleistift in den drei sanften,
              gedämpften Farben Coconut Milk, Rose Shadows und Dapple Gray –
              perfekt für die vielen Zwischentöne in Deinem Alltag.
            </div>
            <a href=""> Mehr erfahren </a>
          </div>
        </div>
      </div>
    </Slide>

    <template #addons>
      <Navigation />
      <Pagination />
    </template>
  </Carousel>
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
.slider {
  display: flex;
  justify-content: center;
  width: 99%;
  height: 420px;
  margin-top: 0px;
  padding-right: 15px;

  .header {
    display: table-cell;
    height: 100%;
    position: relative;
    vertical-align: top;
    width: 100%;
    z-index: 0;
    img {
      max-height: 400px;
      height: 100%;
    }
  }
  .body {
    box-shadow: 0 1px 1px 1px rgb(0 0 0 / 18%);
    user-select: none;
    background-color: #ffffff;
    cursor: default;
    display: table-cell;
    float: right;
    height: inherit;
    padding: 0 50px 0 37px;
    position: relative;
    vertical-align: top;
    width: 97%;
    height: 400px;
    z-index: 1005;
    cursor: pointer;
    margin-top: 10px 0;
    .title {
      overflow: hidden;
      max-height: 93px;
      color: #05301a;
      font-family: "Times New Roman", Times, serif;
      font-size: 28px;
      letter-spacing: 0.01em;
      line-height: 31px;
      margin-top: 45px;
      position: relative;
    }
    .description {
      margin-top: 18px;
      overflow: hidden;
      position: relative;
      max-height: 126px;
      color: #707170;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 14px;
      letter-spacing: 0.035em;
      line-height: 21px;
    }
    a {
      border-radius: 3px;
      background: #05301a;
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
    }
    a:hover {
      opacity: 0.8s;
      background: #6b8276;
    }
  }
  .body::before {
    box-shadow: 0 1px 1px 1px rgb(0 0 0 / 20%);
    transition: all 0.2s linear;
    transform: rotate(-1.5deg);
    left: -6px;
    top: 0;
    z-index: -1;
    background-color: #ffffff;
    content: "";
    height: 100%;
    position: absolute;
    width: 100%;
  }
  .body:hover::before {
    transform: rotate(-5deg);
  }
  .body:hover::after {
    transform: rotate(3deg);
  }
  .body::after {
    box-shadow: 0 1px 1px 1px rgb(0 0 0 / 20%);
    transition: all 0.2s linear;
    transform: rotate(-3.5deg);
    left: -6px;
    top: 0;
    z-index: -1;
    background-color: #ffffff;
    content: "";
    height: 100%;
    position: absolute;
    width: 100%;
  }
}
.carousel {
  width: 1280px;
  height: 500px;
  margin: 0 auto;

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
  top: 80%;
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
  right: 30px;
  position: absolute;
  top: 50%;
  height: 58px;
  margin-top: 0;
  width: 40px;
}

.carousel__prev {
  background-color: transparent;
  position: absolute;
  top: 50%;
  height: 58px;
  margin-top: 0;
  width: 40px;
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
</style>
