<template>
  <div>
    <h1>Asset Injest on PI Server</h1>
    <div class="log-panel">
      <div class="logs">
        <p v-bind:key="log" v-for="log in logs">{{ log }}<br /></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AssetIntake",
  data() {
    return {
      logs: ["test", "test", "test", "test", "test", "test"],
    };
  },
  mounted() {
    // async program command to PI
    // log retrieved info to screen by saving to logs[]
  },
};
</script>

<style scoped>
.log-panel {
  background: #fff;
  width: 50%;
  border-radius: 2rem;
}

.logs {
  width: 90%;
  text-align: left;
  margin-left: 40px;
  margin-top: 20px;
}
</style>
