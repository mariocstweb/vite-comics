<script>
import MainContent from './MainContent.vue'
export default {
  name: "AppMain",
  components: {
    MainContent
  },
  props: {
    series: Array
  }
};
</script>

<template>
  <main>
    <div class="jumbotron">
      <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
    <div>
      <button class="series-btn">CURRENT SERIES</button>
      <div class="card-container">
        <MainContent v-for="serie in series" :thumb="serie.thumb" :series="serie.series" />
      </div>
    </div>
    <div class="btn-container">
      <button class="load-btn">LOAD MORE</button>
    </div>
  </main>
</template>

<style leng="scss" scoped>
main {
  background-color: #1C1C1C;
  position: relative;
}

.jumbotron {
  height: 400px;
  overflow: hidden;

  img {
    width: 100%;
    height: auto;

  }
}

.series-btn {
  background-color: #0282F9;
  padding: 10px 30px;
  border: 0;
  color: white;
  font-weight: bolder;
  position: absolute;

  top: 34.5%;
  left: 24%;
  transform: translate(-50%, -50%);
}

h2 {
  margin: 0;
}

.card-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 30px;
}

.series-card {
  flex-basis: calc((100% / 6) - 20px);
}


.btn-container {
  display: flex;
  justify-content: center;

  .load-btn {
    background-color: #0282F9;
    padding: 10px 30px;
    border: 0;
    color: white;
    margin-bottom: 30px;
  }
}
</style>
