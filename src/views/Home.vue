<template>
  <div id="main">
    <h1>Starting Window</h1>
    <p>Please choose an available option below to proceed with an action</p>
    <p class="disclaimer">Buttons will redirect you to a new page</p>
    <br />
    <div class="buttons">
      <Button class="injest" title="SD-Card Injest on PI" @click="toInjest" />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Button from "@/components/Button.vue";

export default {
  name: "Home",
  components: {
    Button,
  },
  methods: {
    toInjest() {
      this.$router.push("/asset-intake");
    },
  },
};
</script>

<style scoped>
.buttons {
  margin: 1% 5%;
}

.disclaimer {
  font-style: italic;
}
</style>
