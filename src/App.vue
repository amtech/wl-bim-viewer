<template>
  <div id="app">
    <div class="a-logo">
      <a href="http://github.com/hql7">Github</a>&nbsp;
      <a href="17796646068@163.com">Email</a>
      <img alt="Vue logo" class="a-img" src="./assets/logo.png" />
      <a href="https://segmentfault.com/u/weilan_595deafa69d76">Segmentfault</a>&nbsp;
      <a href="https://juejin.im/user/591d141e0ce46300692184a4">掘金</a>
    </div>
    <!-- viewer区 -->
    <wl-viewer multiple :docs="bims" class="wl-viewer"></wl-viewer>
  </div>
</template>

<script>
import wlViewer from "@/pages/cad-viewer";

export default {
  name: "App",
  components: {
    wlViewer
  },
  data() {
    return {
      bims: [
        {
          name: "urn_model1",
          path: "bim/1/0.svf",
          modelObj: null
        },
        {
          name: "urn_model2",
          path: "bim/2/0.svf",
          modelObj: null
        },
        {
          name: "urn_model3",
          path: "bim/3/0.svf",
          modelObj: null
        },
        {
          name: "urn_model4",
          path: "bim/4/0.svf",
          modelObj: null
        },
        {
          name: "urn_model5",
          path: "bim/6/Sphere.svf",
          modelObj: null
        },
        {
          name: "urn_model6",
          path: "bim/6/Sphere.svf",
          modelObj: null
        }
      ]
    };
  }
};
</script>

<style lang="scss">
html,
body {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
  width: 100%;
}

.a-logo {
  height: 20%;
  margin-bottom: 1%;

  > .a-img {
    height: 100%;
  }
}

.wl-viewer {
  width: 90%;
  height: 75%;
  margin: 0 auto;
}
</style>
