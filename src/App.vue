<template>
  <div id="app">
    <header>
      <div class="navbar-fixed">
        <nav>
          <div class="nav-wrapper pl-2 teal lighten-2">
            <a href="#" class="brand-logo">MyCompany</a>
            <a href="#" data-target="mobile-demo" class="sidenav-trigger"
              ><i class="material-icons">menu</i></a
            >
            <ul id="nav-mobile" class="right hide-on-med-and-down">
              <li>
                <router-link to="/" class="nav-item r-item">Home</router-link>
              </li>
              <li>
                <router-link to="faq" class="nav-item r-item"
                  >Features</router-link
                >
              </li>
              <li>
                <router-link to="faq" class="nav-item r-item"
                  >About</router-link
                >
              </li>
              <li>
                <router-link to="faq" class="nav-item r-item">FAQ</router-link>
              </li>
              <li>
                <a class="waves-effect waves-light btn-small"
                  ><i class="material-icons left">thumb_up</i>JOIN NOW</a
                >
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </header>
    <ul class="sidenav" id="mobile-demo">
      <li>
        <router-link to="/" class="nav-item r-item">Home</router-link>
      </li>
      <li>
        <router-link to="faq" class="nav-item r-item">Features</router-link>
      </li>
      <li>
        <router-link to="faq" class="nav-item r-item">About</router-link>
      </li>
      <li>
        <router-link to="faq" class="nav-item r-item">FAQ</router-link>
      </li>
    </ul>

    <router-view></router-view>

    <footer class="page-footer teal lighten-2">
      <div class="container">
        <div class="row">
          <div class="col l10 s12">
            <h5 class="white-text">Footer Content</h5>
          </div>
          <div class="col l2 s12">
            <div class="">
              <a>
                <font-awesome-icon
                  :icon="['fab', 'facebook']"
                  size="3x"
                  class="white-text"
                />
              </a>
              <a>
                <font-awesome-icon
                  :icon="['fab', 'twitter']"
                  size="3x"
                  class="white-text"
                />
              </a>
            </div>
          </div>
        </div>

        <div class="row">
          <div class="col l12 s12">
            whatever you want your footer to show goes here
          </div>
        </div>
      </div>
      <div class="footer-copyright">
        <div class="container">
          <div class="center-align">
            © 2021 visuAll
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import $ from "jquery";
import M from "materialize-css";

export default {
  name: "App",
  mounted() {
    M.AutoInit();
  }
};

// $(document).ready(function() {
//   $(".sidenav").sidenav();
// });

document.addEventListener("DOMContentLoaded", function() {
  var elems = document.querySelectorAll(".sidenav");
  var instances = M.Sidenav.init(elems, {});
});
</script>

<style src="./styles/style.css" lang="css">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #0e4b34;
  margin-top: 60px;
}
</style>
