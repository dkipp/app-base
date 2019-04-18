<template>
  <div id="app">
    <activity-bar id="activityBar" v-model="sidebarTab"></activity-bar>
    <side-bar id="sideBar" :selected="sidebarTab"></side-bar>
    <!--div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div-->
    <router-view id="main" />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import ActivityBar from '@/components/ActivityBar.vue';
import SideBar from '@/components/SideBar.vue';

@Component({
  components: {
    ActivityBar,
    SideBar,
  },
})
export default class App extends Vue {
  @Prop() public sidebarTab: string  = 'tab2';
}

</script>

<style lang="scss">
@import '../node_modules/@adobe/spectrum-css/dist/spectrum-core.css';
@import '../node_modules/@adobe/spectrum-css/dist/spectrum-light.css';

body {
  margin: 0;
}

#app {
  display: grid;
  grid: "menuBar menuBar menuBar" auto
      "activityBar sideBar main" 1fr
      "statusBar statusBar statusBar" auto
      / auto 260px 1fr;
  box-sizing: border-box;
  width: 100vw;
  height: 100vh;
}

#activityBar{
  grid-area: activityBar;
  border-right: 1px solid rgba(0,0,0, .06);
  background-color: rgba(0,0,0, .02);
  padding: .2em;
}

#sideBar{
  grid-area: sideBar;
}

#main{
  grid-area: main;
  overflow: hidden;
}
</style>
