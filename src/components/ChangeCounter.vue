<template>
  <button @click="increment">Add 10</button>
  <button @click="increase({ value: 20 })">Add 10</button>
</template>

<script>
import { mapActions } from 'vuex';

export default {
  methods: {
    // addOne() {
    //   this.$store.dispatch('increase', { value: 10 });
    // },
    ...mapActions(['increment', 'increase']),
  },
};
</script>
