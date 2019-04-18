<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/human.png" style="filter: brightness(96%);">
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import VuesaActionButton from '@/components/vuesa/ActionButton.vue';

@Component({
  components: {
    HelloWorld,
    VuesaActionButton,
  },
})
export default class Home extends Vue {}
</script>
