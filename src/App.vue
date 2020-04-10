<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 vcenter">
        <button @click="selectedComponent = 'app-quote'">Select quote</button>
        <button @click="selectedComponent = 'app-author'">Select author</button>
        <hr />
        <component :is="selectedComponent"></component>
        <!-- <app-quote>
          <h2 slot="title">{{ quoteTitle }}</h2>
          <p slot="content">A wonderful quote!</p>
        </app-quote>-->
      </div>
    </div>
  </div>
</template>

<script>
import Quote from "./components/Quote.vue";
import Author from "./components/Author.vue";

export default {
  data() {
    return {
      quoteTitle: "The quote",
      selectedComponent: "app-quote"
    };
  },
  components: {
    "app-quote": Quote,
    "app-author": Author
  }
};
</script>

<style>
</style>
