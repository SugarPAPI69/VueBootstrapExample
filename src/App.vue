<template>
  <div id="app">
    <div class="page" v-if="getSpinner">
      <b-spinner class="spinner" :variant="'primary'" :key="'primary'"></b-spinner>
    </div>
    <div id="nav">
      <top-header></top-header>
    </div>
    <router-view />
  </div>
</template>
<script>
import TopHeader from "@/components/top-header.vue";
import { mapGetters } from "vuex";
export default {
  components: { "top-header": TopHeader },
  computed: {
    ...mapGetters(["getSpinner"])
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #21231f;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #FFFFFF;

    &.router-link-exact-active {
      color: #21231f;
    }
  }
}
.page {
  position: absolute;
  background: rgba(0, 0, 0, 0.3);
  z-index: 25;
  width: 100%;
  height: 100%;
}
.spinner {
  z-index: 26;
  position: relative;
  top: 50%;
}

body {
  background: #eefa84;
  padding: 0;
  margin: 0;
}
</style>
