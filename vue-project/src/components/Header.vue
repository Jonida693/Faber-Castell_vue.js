<template>
  <header>
    <section class="navigation">
      <div class="header-nav">
        <div class="navbar">
          <div class="shipping-info">{{ shipingInfo }}</div>
          <nav class="nav">
            <ul>
              <li>Our Product</li>
              <li>Tutorials</li>
              <li>Company</li>
              <li class="arrow"></li>
            </ul>
          </nav>
        </div>
        <div>
          <a class="logo" href="">
            <img
              src="https://www.faber-castell.com/-/media/Faber-Castell-new/icons/faber-castell.ashx?h=62&w=195&la=en-Glob&hash=FD9B2D356EFBE33BCC903C0B60FCC44536FD6820"
              alt=""
            />
          </a>
        </div>
        <div class="">
          <div class="meta">
            <ul>
              <li>Press</li>
              <li>Service & Help</li>
              <li>Country Selector</li>
            </ul>
          </div>

          <div class="shop-menu">
            <ul>
              <li class="search">
                <svg
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  width="25"
                  height="30"
                  viewBox="0 0 32 32"
                >
                  <path
                    d="M13.455 2.182c6.226 0 11.273 5.047 11.273 11.273 0 2.851-1.058 5.454-2.803 7.439l7.483 7.485-1.029 1.029-7.485-7.483c-1.985 1.745-4.588 2.803-7.439 2.803-6.226 0-11.273-5.047-11.273-11.273s5.047-11.273 11.273-11.273zM13.455 3.636c-5.422 0-9.818 4.396-9.818 9.818s4.396 9.818 9.818 9.818c5.422 0 9.818-4.396 9.818-9.818s-4.396-9.818-9.818-9.818z"
                  ></path>
                </svg>
              </li>
              <li class="acc-menu">
                <svg
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  width="25"
                  height="30"
                  viewBox="0 0 32 32"
                >
                  <path
                    d="M16 2.909c7.23 0 13.091 5.861 13.091 13.091s-5.861 13.091-13.091 13.091c-7.23 0-13.091-5.861-13.091-13.091s5.861-13.091 13.091-13.091zM18.181 21.818h-3.631c-1.576 0-3.036 0.704-4.013 1.933-0.468 0.589-0.79 1.252-0.954 1.958 1.841 1.218 4.046 1.927 6.417 1.927 2.639 0 5.073-0.879 7.025-2.359-0.355-1.074-1.075-2.004-2.058-2.639-0.767-0.495-1.647-0.775-2.558-0.815l-0.228-0.005zM16 4.364c-6.427 0-11.636 5.21-11.636 11.636 0 3.495 1.54 6.629 3.979 8.762 0.235-0.686 0.59-1.332 1.055-1.917 1.207-1.518 2.994-2.414 4.928-2.478l0.224-0.004h3.631c1.271 0 2.509 0.364 3.575 1.053 1.090 0.703 1.932 1.694 2.437 2.846 2.126-2.108 3.443-5.032 3.443-8.263 0-6.427-5.21-11.636-11.636-11.636zM16 7.273c3.209 0 5.818 2.609 5.818 5.818s-2.609 5.818-5.818 5.818c-3.208 0-5.818-2.61-5.818-5.818 0-3.209 2.609-5.818 5.818-5.818zM16 8.727c-2.406 0-4.364 1.958-4.364 4.364s1.959 4.364 4.364 4.364c2.406 0 4.364-1.958 4.364-4.364s-1.958-4.364-4.364-4.364z"
                  ></path>
                </svg>
              </li>
              <li class="cart">
                <svg
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  width="25"
                  height="30"
                  viewBox="0 0 32 32"
                >
                  <path
                    d="M16 2.182c3.213 0 5.818 2.605 5.818 5.818v1.455h2.909l2.182 19.636h-21.818l2.182-19.636h2.909v-1.455c0-3.213 2.605-5.818 5.818-5.818zM23.425 10.909h-14.852l-1.858 16.727h18.568l-1.858-16.727zM16 3.636c-2.355 0-4.275 1.866-4.361 4.2l-0.003 0.164v1.455h8.727v-1.455c0-2.41-1.953-4.364-4.364-4.364z"
                  ></path>
                </svg>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </header>
</template>
<script>
import navMenu from "./navMenu.vue";

export default {
  data: () => {
    return {
      shipingInfo: "Versandkostenfrei ab 39€",
    };
  },
  methods: {},
  components: {
    navMenu,
  },
};
</script>

<style lang="scss">
header {
  width: 100%;
  background: #05301a;
  height: 135px;
  .navigation {
    max-width: 1280px;
    margin: 0 auto;
    height: 135px;
    .header-nav {
      display: flex;
      justify-content: space-between;
      min-height: 65px;
      padding-bottom: 53px;
      position: relative;
      z-index: 1002;
      align-items: center;
      text-align: center;
      > div {
        height: 130px;
      }
      .shipping-info {
        color: #ffffff;
        font-size: 11px;
        letter-spacing: 1.1px;
        line-height: 16px;
        margin-left: 44px;
        padding-top: 5px;
      }
      .active {
        color: red;
      }
      .nav {
        position: absolute;
        bottom: 55px;
        display: flex;
        justify-content: flex-end;
        ul {
          display: flex;
          justify-content: space-between;
          color: #fff;
          list-style: none;
          margin: 0;
          position: relative;

          li:not(:first-of-type) {
            margin-left: 25px;
          }
          .arrow {
            bottom: 15px;
            position: absolute;
            cursor: pointer;
            font-stretch: 100%;
            z-index: 1204;
          }

          .arrow::after {
            // border-color: #ffffff;
            border-bottom-color: #ffffff !important;
            border-width: 8px;
            margin-left: -8px;
            border: 15px solid transparent;
            bottom: -23px;
            content: " ";
            height: 0px;
            left: 55%;
            pointer-events: none;
            position: absolute;
            width: 0;
          }
        }
      }
      .meta {
        display: flex;
        justify-content: flex-end;
        font-size: 11px;
        letter-spacing: 1.1px;
        line-height: 16px;
        margin-left: 44px;
        padding-top: 5px;

        ul {
          display: flex;
          justify-content: space-between;
          color: #b8ddc0;
          list-style: none;
          margin: 0;

          li:not(:first-of-type) {
            margin-left: 25px;
          }
        }
      }
      .logo {
        position: relative;
        display: inline-block;
        text-align: center;
        width: 100%;
      }
      img {
        position: absolute;
        transform: translateX(5%);
        height: auto;
        max-width: 195px;
      }
    }
    .shop-menu {
      color: #fff;
      cursor: pointer;
      fill: #fff;
      bottom: 50px;
      position: absolute;
      right: 0px;

      ul {
        display: inline-flex;
        vertical-align: baseline;
        list-style: none;
        li {
          float: left;
          margin: 0 13px;
          position: relative;
        }
      }
    }
  }
}
</style>
