<script >
import Card from "./components/Card.vue"
export default {
  components: {
    Card
  },
  data() {
    return{
      a:1,
      temp:98
    }
  },
  methods: {
    changeAValue(){
      this.a=this.temp
    }
  },
  mounted() {

    this.a = 2;
  }
}
</script>

<template>
  
    <!-- <p>{{ a }}</p> -->
    <!-- <card /> -->
    <div class="text-area">
      <h1>V-model</h1>
      <h1>V-on</h1>
      <h2>a: {{ a }}</h2>
      <p>temp: {{ temp }}</p>
      <input type="number" v-model="temp">
      <button type="button" v-on:click="changeAValue">update</button>
    </div>
  

</template>

<style lang="scss" scoped>
  .text-area{
    text-align: center;
  }
</style>
