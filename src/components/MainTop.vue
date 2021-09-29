<template>
  <main>
    <div class="container">
      <h2> --> Content goes here</h2>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainTop'
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