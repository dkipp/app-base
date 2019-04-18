<template>
  <div style="margin:auto 1em; ">


<div class="spectrum-Tabs spectrum-Tabs--horizontal">
  <div class="spectrum-Tabs-item" tabindex="0">
    <label class="spectrum-Tabs-itemLabel">Tab 1</label>
  </div>
  <div class="spectrum-Tabs-item" tabindex="0">
    <label class="spectrum-Tabs-itemLabel">Tab 2</label>
  </div>
  <div class="spectrum-Tabs-item is-selected" tabindex="0">
    <label class="spectrum-Tabs-itemLabel">Tab 3</label>
  </div>
  <div class="spectrum-Tabs-item" tabindex="0">
    <label class="spectrum-Tabs-itemLabel">Tab 4</label>
  </div>
  <div class="spectrum-Tabs-selectionIndicator" style="width: 37px; left: 115px;"></div>
</div>
<br />

    <div class="spectrum-ButtonGroup">
      <vuesa-action-button quiet icon="spectrum-icons.svg#spectrum-icon-18-AlignTop"></vuesa-action-button>
      <vuesa-action-button quiet icon="spectrum-icons.svg#spectrum-icon-18-AlignMiddle"></vuesa-action-button>
      <vuesa-action-button quiet icon="spectrum-icons.svg#spectrum-icon-18-AlignBottom"></vuesa-action-button>
      <vuesa-action-button quiet icon="spectrum-icons.svg#spectrum-icon-18-DistributeHorizontally" disabled></vuesa-action-button>
    </div>
    <vuesa-rule></vuesa-rule>
    <div class="spectrum-Slider spectrum-Slider--color">
      <div class="spectrum-Slider-labelContainer">
        <label class="spectrum-Slider-label" id="spectrum-Slider--color-label-0" for="spectrum-Slider--color-input-0">Color</label>
        <div class="spectrum-Slider-value" role="textbox" aria-readonly="true" aria-labelledby="spectrum-Slider--color-label-0">#2680eb</div>
      </div>
      <div class="spectrum-Slider-controls">
        <div class="spectrum-Slider-track" style="background: linear-gradient(to right, rgb(38, 128, 235), rgb(9, 90, 186))"></div>
        <div class="spectrum-Slider-handle" style="left: 40%;">
          <input type="range" class="spectrum-Slider-input" value="14" aria-valuetext="#2680eb" step="2" min="10" max="20" id="spectrum-Slider--color-input-0">
        </div>
      </div>
    </div>
    <vuesa-rule></vuesa-rule>
    <div class="spectrum-Slider spectrum-Slider--ramp">
      <div class="spectrum-Slider-labelContainer">
        <label class="spectrum-Slider-label" id="spectrum-Slider-label-10" for="spectrum-Slider-input-10">Slider Label</label>
        <div class="spectrum-Slider-value" role="textbox" aria-readonly="true" aria-labelledby="spectrum-Slider-label-10">14</div>
      </div>
      <div class="spectrum-Slider-controls">
        <div class="spectrum-Slider-ramp">
          <svg viewBox="0 0 240 16" preserveAspectRatio="none" aria-hidden="true" focusable="false">
            <path d="M240,4v8c0,2.3-1.9,4.1-4.2,4L1,9C0.4,9,0,8.5,0,8c0-0.5,0.4-1,1-1l234.8-7C238.1-0.1,240,1.7,240,4z"></path>
          </svg>
        </div>
        <div class="spectrum-Slider-handle" style="left: 40%;">
          <input type="range" class="spectrum-Slider-input" value="14" step="2" min="10" max="20" id="spectrum-Slider-input-10">
        </div>
      </div>
    </div>
    <vuesa-rule></vuesa-rule>
    <div class="spectrum-Slider spectrum-Slider--range" role="group" aria-labelledby="spectrum-Slider-label-4">
      <div class="spectrum-Slider-labelContainer" role="presentation">
        <label class="spectrum-Slider-label" id="spectrum-Slider-label-4" for="spectrum-Slider-input-4-0">Slider Label</label>
        <div class="spectrum-Slider-value" role="textbox" aria-readonly="true" aria-labelledby="spectrum-Slider-label-4">14 - 48</div>
      </div>
      <div class="spectrum-Slider-controls" role="presentation">
        <div class="spectrum-Slider-track" style="width: 20%;"></div>
        <div class="spectrum-Slider-handle" style="left: 20%;" role="presentation">
          <input type="range" class="spectrum-Slider-input" value="14" step="2" min="10" max="20" aria-label="min" id="spectrum-Slider-input-4-0" aria-labelledby="spectrum-Slider-label-4 spectrum-Slider-input-4-0">
        </div>
        <div class="spectrum-Slider-track" style="left: 20%; right: 40%;"></div>
        <div class="spectrum-Slider-handle" style="left: 60%;" role="presentation">
          <input type="range" class="spectrum-Slider-input" value="14" step="2" min="10" max="20" aria-label="max" id="spectrum-Slider-input-4-1" aria-labelledby="spectrum-Slider-label-4 spectrum-Slider-input-4-1">
        </div>
        <div class="spectrum-Slider-track" style="width: 40%;"></div>
      </div>
    </div>
    <vuesa-rule></vuesa-rule>
    <div class="spectrum-ToggleSwitch">
      <input type="checkbox" class="spectrum-ToggleSwitch-input" id="toggle-onoff-0">
      <span class="spectrum-ToggleSwitch-switch"></span>
      <label class="spectrum-ToggleSwitch-label" for="toggle-onoff-0">Toggle Off</label>
    </div>
    <div class="spectrum-ToggleSwitch">
      <input type="checkbox" class="spectrum-ToggleSwitch-input" id="toggle-onoff-1" checked>
      <span class="spectrum-ToggleSwitch-switch"></span>
      <label class="spectrum-ToggleSwitch-label" for="toggle-onoff-1">Toggle On</label>
    </div>

  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import VuesaActionButton from '@/components/vuesa/ActionButton.vue';
import VuesaRule from '@/components/vuesa/Rule.vue';

@Component({
  components: {
    VuesaActionButton,
    VuesaRule,
  },
})
export default class SideBarOne extends Vue {
  // @Prop() private selected!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
