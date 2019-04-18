<template>
  <ul class="spectrum-TreeView" style="width: 250px">
    <li class="spectrum-TreeView-item">
      <a class="spectrum-TreeView-itemLink" href="#">
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
        Layer 1
      </a>
    </li>

    <li class="spectrum-TreeView-item is-open">
      <a class="spectrum-TreeView-itemLink" href="#">
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-ChevronRight"></vuesa-icon>
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Folder"></vuesa-icon>
        Group 1
      </a>
      <ul class="spectrum-TreeView">
        <li class="spectrum-TreeView-item">
          <a class="spectrum-TreeView-itemLink" href="#">
            <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
            Layer 2
          </a>
        </li>
        <li class="spectrum-TreeView-item">
          <a class="spectrum-TreeView-itemLink" href="#">
            <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
            Layer 3
          </a>
        </li>
      </ul>
    </li>

    <li class="spectrum-TreeView-item">
      <a class="spectrum-TreeView-itemLink" href="#">
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
        Layer 4
      </a>
    </li>
    <li class="spectrum-TreeView-item">
      <a class="spectrum-TreeView-itemLink" href="#">
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
        Layer 5
      </a>
    </li>

    <li class="spectrum-TreeView-item is-open">
      <a class="spectrum-TreeView-itemLink" href="#">
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-ChevronRight"></vuesa-icon>
        <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Folder"></vuesa-icon>
        Group 2
      </a>
      <ul class="spectrum-TreeView">
        <li class="spectrum-TreeView-item is-open">
          <a class="spectrum-TreeView-itemLink" href="#">
            <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-ChevronRight"></vuesa-icon>
            <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Folder"></vuesa-icon>
            Group 3
          </a>
          <ul class="spectrum-TreeView">
            <li class="spectrum-TreeView-item">
              <a class="spectrum-TreeView-itemLink" href="#">
                <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-ChevronRight"></vuesa-icon>
                <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Folder"></vuesa-icon>
                Group 4
              </a>
              <ul class="spectrum-TreeView">
                <li class="spectrum-TreeView-item">
                  <a class="spectrum-TreeView-itemLink" href="#">
                    <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Layers"></vuesa-icon>
                    Layer 6
                  </a>
                </li>
                <li class="spectrum-TreeView-item">
                  <a class="spectrum-TreeView-itemLink" href="#">
                    <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-ChevronRight"></vuesa-icon>
                    <vuesa-icon icon="spectrum-icons.svg#spectrum-icon-18-Folder"></vuesa-icon>
                    Group 5
                  </a>
                </li>
              </ul>
            </li>
          </ul>
        </li>
      </ul>
    </li>
  </ul>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import VuesaIcon from '@/components/vuesa/Icon.vue';

@Component({
  components: {
    VuesaIcon,
  },
})
export default class SideBarTwo extends Vue {
  // @Prop() private selected!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
