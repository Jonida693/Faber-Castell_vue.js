<template>
  <section class="stage-galery">
    <!-- <slick ref="slick">
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
    </slick> -->

    <!-- <div id="slide">
      <gile :initial-slide="1"
        ><img
          class="slide"
          src="https://images.unsplash.com/photo-1506260408121-e353d10b87c7?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1523712999610-f77fbcfc3843?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1524260855046-f743b3cdad07?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1526080676457-4544bf0ebba9?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1519681393784-d120267933ba?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1426170042593-200f250dfdaf?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        /><img
          class="slide"
          src="https://images.unsplash.com/photo-1529815481058-55e5b656f6d6?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1600&amp;fit=max&amp;ixid=eyJhcHBfaWQiOjE0NTg5fQ"
        />
        <template>
          <slot name="prevButton">
            <i class="fas fa-chevron-left"></i>
          </slot>
        </template>
        <template>
          <slot name="nextButton">
            <i class="fas fa-chevron-right"></i>
          </slot>
        </template>
      </gile>
    </div> -->

    <agile ref="carousel">
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

      <div class="slide">
        <h3>slide 2</h3>
      </div>
    </agile>
  </section>
</template>

<script>
// import VueSlickCarousel from "vue-slick-carousel";
// import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
// import { Carousel, Slide } from "vue-carousel";
// import { def } from "@vue/shared";
// import Slick from "vue-slick";
// import "/node_modules/slick-carousel/slick/slick-theme.scss";
// export default {
//   data() {
//     return {
//       slickOptions: {
//         slidesToShow: 3,
//         // Any other options that can be got from plugin documentation
//       },
//     };
//   },
//   methods: {},
//   components: { Slick },
// };
</script>

<style lang="scss">
.agile {
  &__nav-button {
    background: transparent;
    border: none;
    color: #fff;
    cursor: pointer;
    font-size: 24px;
    height: 100%;
    position: absolute;
    top: 0;
    transition-duration: 0.3s;
    width: 80px;
  }

  &:hover {
    background-color: rgba(#000, 0.5);
    opacity: 1;
  }

  &--prev {
    left: 0;
  }

  &--next {
    right: 0;
  }

  &__dots {
    bottom: 10px;
    left: 50%;
    position: absolute;
    transform: translateX(-50%);
  }

  &__dot {
    margin: 0 10px;
  }

  button {
    background-color: transparent;
    border: 1px solid #fff;
    border-radius: 50%;
    cursor: pointer;
    display: block;
    height: 10px;
    font-size: 0;
    line-height: 0;
    margin: 0;
    padding: 0;
    transition-duration: 0.3s;
    width: 10px;
  }

  &--current,
  &:hover {
    button {
      background-color: #fff;
    }
  }
}

// Slides styles
.slide {
  display: block;
  height: 500px;
  object-fit: cover;
  width: 100%;
}
.stage-galery {
  max-width: 1280px;
  max-height: 400px;
  margin: 0 auto;

  .slider {
    display: flex;
    justify-content: center;
    width: 100%;
    margin-bottom: 20px;
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
      width: 100%;
      height: 400px;
      z-index: 1;
      cursor: pointer;
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
}
</style>
