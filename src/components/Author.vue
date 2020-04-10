<template>
  <div>
    <h3>The author</h3>
    <button @click="score++">Vote</button>
    <p>{{ score }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      score: 0
    };
  }
};
</script>