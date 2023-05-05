<script >
export default {
  components: {

  },
  data() {
    return {
      isShow: true
    }
  },
  methods: {
    switchBoo() {
      this.isShow = !this.isShow
    }
  },
  mounted() {

  }
}
</script>

<template>
  <div class="text-area">
    <h1>V-model</h1>
    <button type="button" v-on:click="switchBoo">switch</button>
    <p>{{ isShow }}</p>
    <div v-if="isShow" class="box bg-primary"></div>
    <div v-else class="box bg-info"></div>
  </div>
</template>

<style lang="scss" scoped>
.text-area {
  text-align: center;
}

.box {
  width: 50px;
  height: 50px;
}
</style>
