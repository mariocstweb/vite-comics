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
  height: 260px;
  margin-bottom: 60px;

  img {
    max-width: 100%;
    height: 100%;
    margin-bottom: 10px;
    object-fit: cover
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