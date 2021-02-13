<template>
  <div class="main">
    <div class="button">
      <h1>{{ title }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: {
    title: String,
  },
};
</script>

<style scoped>
.button {
  width: 11rem;
  height: 5rem;
  background-image: linear-gradient(to bottom right, #1f6eff, #43e9e1);
  padding: 0.5rem 1.5rem;
  border-radius: 1rem;
  border: 3px solid white;
  cursor: pointer;
}

h1 {
  font-size: 1.5em;
  display: inline-block;
}
</style>
