<template>
  <button class="spectrum-ActionButton" :class="{ 'spectrum-ActionButton--quiet': quiet, 'is-selected': selected }" :disabled="disabled">
    <vuesa-icon v-if="icon" v-bind:icon="icon"></vuesa-icon>
    <span v-if="$slots.default" class="spectrum-ActionButton-label"><slot></slot></span>
  </button>
</template>
<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import VuesaIcon from '@/components/vuesa/Icon.vue';

@Component({
  components: {
    VuesaIcon,
  },
})
export default class VuesaActionButton extends Vue {
  @Prop(Boolean) public selected!: boolean;
  @Prop(Boolean) public quiet!: boolean;
  @Prop(Boolean) public disabled!: boolean;
  @Prop(String) public icon!: string;
}
</script>