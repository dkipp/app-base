<template>
  <div class="spectrum-ButtonGroup spectrum-ButtonGroup--vertical">
    <vuesa-action-button @click.native="$emit('change', 'tab1')" :selected="(checked=='tab1')" quiet icon="spectrum-icons.svg#spectrum-icon-24-Demographic"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab2')" :selected="(checked=='tab2')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Properties"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab3')" :selected="(checked=='tab3')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Edit"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab4')" :selected="(checked=='tab4')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Edit"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab5')" :selected="(checked=='tab5')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Edit"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab6')" :selected="(checked=='tab6')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Edit"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab7')" :selected="(checked=='tab7')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Gears" style="margin-top:auto"></vuesa-action-button>
    <vuesa-action-button @click.native="$emit('change', 'tab8')" :selected="(checked=='tab8')" quiet icon="spectrum-icons.svg#spectrum-icon-18-Settings"></vuesa-action-button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Model, Vue } from 'vue-property-decorator';
import VuesaActionButton from '@/components/vuesa/ActionButton.vue';

@Component({
  components: {
    VuesaActionButton,
  },
})
export default class ActivityBar extends Vue {
  @Model('change', { type: String }) public readonly checked!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
