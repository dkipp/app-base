<template>
  <svg class="spectrum-Icon spectrum-Icon--sizeS" focusable="false" aria-hidden="true" aria-label="label">
    <use :xlink:href="icon" />
  </svg>
</template>
<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class VuesaIcon extends Vue {
  @Prop(String) public icon!: string;
  @Prop(String) public size!: string;
  @Prop(String) public label!: string;
}
</script>