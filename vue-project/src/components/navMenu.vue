<template>
  <div id="flyouts">
    <div class="wrap">
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/">{{tittle}}</a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Spielen & Lemen </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Art & Graphic </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Creative Studio </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Allgemens Schreiben & Markieren </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Fine Writing </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Geschenkefinder </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Sale </a>
        </li>
      </ul>
      <ul class="dropdown-menu">
        <li>
          <a class="title" href="/"> Gravur </a>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  data: () => {
    return {
      tittle: "Alle Produkte",
    };
  },
};
</script>
<style lang="scss">
#flyouts {
  background: #ffffff;
  border-bottom: 1px solid #dadada;
  box-shadow: 0 1px 0 #ebebe6;
  display: block;
  float: left;
  position: relative;
  width: 100%;
  font-size: 14px;
  height: 52px;
  z-index: 1003;
  .wrap {
    max-width: 1280px;
    width: 100%;
    padding-left: 30px;
    margin: 0 auto;
    .dropdown-menu {
      box-sizing: border-box;
      list-style-type: none;
      padding: 0 20px;
      float: left;
      li {
        text-decoration: none;
        list-style-type: none;
        color: #707170;
      }
    }
    // .title:hover {
    //   cursor: pointer;
    //   color: #05301a;
    // }
    .dropdown-menu:first-of-type {
      li {
        color: #05301a;
      }
    }
  }
}
</style>
