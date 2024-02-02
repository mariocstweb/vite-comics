<script>
import MainContent from './MainContent.vue'
export default {
  name: "AppMain",
  components: {
    MainContent
  }

};
</script>

<template>
  <main>
    <div class="container">
      <h2>--Content goes here--</h2>
      <div class="card-container">
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
        <MainContent></MainContent>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: #1C1C1C;
  display: flex;
  justify-content: center;
}

h2 {
  margin: 0;
}



.card-container {
  max-width: 1300px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 30px;
}

.series-card {
  flex-basis: calc((100% / 6) - 30px);

}
</style>
