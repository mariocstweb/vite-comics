<script>
export default {
  name: "MainContent",
  props: {
    thumb: String,
    series: String,
  }
};
</script>



<template>
  <div class="series-card">
    <img :src="thumb" :alt="series">
    <p>{{ series }}</p>
  </div>
</template>




<style lang="scss" scoped>
.series-card {

  img {
    max-width: 100%;
    height: auto;
    margin-bottom: 10px
  }

  ;

  p {
    color: white;
    text-transform: uppercase;
    font-weight: 700;
    margin-bottom: 50px;
  }
}
</style>