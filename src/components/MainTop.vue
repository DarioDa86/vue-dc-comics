<template>
  <main>
    <div class="container">
      <Card v-for="(card, index) in comics" :key="index" :prod="card"/>
    </div>
  </main>
</template>

<script>
import Card from '../components/Card.vue';
export default {
  name: 'MainTop',
  components: {
    Card
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';

main{
  background-color: $mainTopBackColor;
  color: #fff;

  .container {

    h2 {
    padding: 30px 0;
    }
  }
}

</style>