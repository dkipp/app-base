<template>
  <div>
    <side-bar-one v-show="selected === 'tab1'"></side-bar-one>
    <side-bar-two v-show="selected === 'tab2'"></side-bar-two>
    <div v-show="selected === 'tab3'">Tab 3</div>
    <div v-show="selected === 'tab4'">Tab 4</div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import VuesaActionButton from '@/components/vuesa/ActionButton.vue';
import SideBarOne from '@/components/SideBarOne.vue';
import SideBarTwo from '@/components/SideBarTwo.vue';

@Component({
  components: {
    VuesaActionButton,
    SideBarOne,
    SideBarTwo,
  },
})
export default class SideBar extends Vue {
  @Prop() private selected!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  vuesa-action-button {
    color: #333;
  }
</style>
