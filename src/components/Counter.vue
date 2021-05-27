<template>
  <div>
    <h2>&#127914; Awesome counter &#10084;</h2>
    <div>{{ counter }}</div>
    <button @click="inc()">+</button>
    <button @click="dec()">-</button>
  </div>
</template>
<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class Counter extends Vue {
    counter = 0;

    inc(): void {
      this.counter += 1;
    }

    dec(): void {
      this.counter -= 1;
    }
}
</script>
