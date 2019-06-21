<template>
    <div id="app">
        <sui-menu :widths="3" color="blue" inverted="true" fixed="bottom">
            <sui-menu-item>
                <icon icon="trash-alt" far class="r1"></icon>
            </sui-menu-item>
            <sui-menu-item>Reviews</sui-menu-item>
            <sui-menu-item active>Upcoming Events</sui-menu-item>
        </sui-menu>
        <div id="nav">
            <router-link to="/">Home</router-link>|
            <router-link to="/about">About</router-link>
        </div>
        <router-view/>
    </div>
</template>

<script>
  import Vue from "vue";
  import SuiVue from "semantic-ui-vue";

  // import "@progress/kendo-ui";
  // import "@progress/kendo-ui/js/messages/kendo.messages.fa-IR.js";

  // import "./assets/css/kendo/kendo.common.min.css";
  // import "./assets/css/kendo/kendo.bootstrap.min.css";
  // import "./assets/css/kendo/kendo.rtl.min.css";

  // import "../node_modules/overlayscrollbars/css/OverlayScrollbars.min.css";
  import "./assets/semantic/dist/components/container.rtl.min.css";
  import "./assets/semantic/dist/components/form.rtl.min.css";
  import "./assets/semantic/dist/components/grid.rtl.min.css";
  import "./assets/semantic/dist/components/input.rtl.min.css";
  import "./assets/semantic/dist/components/label.rtl.css";
  import "./assets/semantic/dist/components/menu.rtl.min.css";
  import "./assets/semantic/dist/components/image.rtl.min.css";
  // import "./assets/semantic/dist/components/placeholder.rtl.css";
  import "./assets/semantic/dist/components/segment.rtl.css";
  import "./assets/semantic/dist/components/list.rtl.css";
  import "./assets/semantic/dist/components/header.rtl.css";
  import "./assets/semantic/dist/components/button.rtl.css";
  import "./assets/semantic/dist/components/card.rtl.css";
  import "./assets/semantic/dist/components/shape.rtl.css";
  import "./assets/semantic/dist/components/checkbox.rtl.css";
  import "./assets/semantic/dist/components/comment.rtl.css";
  import "./assets/semantic/dist/components/dimmer.rtl.css";
  import "./assets/semantic/dist/components/loader.rtl.css";
  import "./assets/css/antd.scss";
  import "./assets/css/semantic.scss";
  // import "../node_modules/mdi/scss/materialdesignicons.scss"
  // import "../node_modules/pretty-checkbox/src/pretty-checkbox.scss"

  // import defaultAvatar from "./assets/images/avatar.png";

  import { library } from "@fortawesome/fontawesome-svg-core";
  import { fas } from "@fortawesome/free-solid-svg-icons";
  import { far } from "@fortawesome/free-regular-svg-icons";
  // import { fab } from '@fortawesome/free-brands-svg-icons'
  import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";

  library.add(far, fas);

  Vue.component("icon", FontAwesomeIcon);

  import "./assets/css/site.scss";

  Vue.use(SuiVue);

  export default {};
</script>

<style lang="scss">
  body {
    padding: 0px;
    margin: 0px;
  }
  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  #nav {
    // padding: 30px;
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>
