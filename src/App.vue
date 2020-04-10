<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 vcenter">
        <app-quote>
          <h2>{{ quoteTitle }}</h2>
          <p>A wonderful quote!</p>
        </app-quote>
      </div>
    </div>
  </div>
</template>

<script>
import Quote from "./components/Quote.vue";

export default {
  data() {
    return {
      quoteTitle: "The quote"
    };
  },
  components: {
    "app-quote": Quote
  }
};
</script>

<style>
</style>
