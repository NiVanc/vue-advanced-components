<template>
  <div>
    <div class="title">
      <slot name="title"></slot>
      <span>
        <slot name="subtitle">The default subtitle</slot>
      </span>
    </div>
    <hr />
    <div>
      <slot name="content"></slot>
    </div>
  </div>
</template>

<script>
</script>

<style scoped>
div {
  border: 1px solid #ccc;
  box-shadow: 1px 1px 5px #ddd;
  margin: 15px auto;
  padding: 35px;
  text-align: center;
}

p {
  margin: 0;
}

.title {
  margin-top: 75px;
}

span {
  font-style: italic;
  color: #666;
}
</style>