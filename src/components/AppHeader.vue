<script>
export default {
  name: "AppHeader",
  data: () => ({
    menuItems: [
      {
        text: 'Characters',
        url: '#',
        current: false,
      },
      {
        text: 'Comics',
        url: '#',
        current: true,
      },
      {
        text: 'Movies',
        url: '#',
        current: false,
      },
      {
        text: 'TV',
        url: '#',
        current: false,
      },
      {
        text: 'Games',
        url: '#',
        current: false,
      },
      {
        text: 'Collectibles',
        url: '#',
        current: false,
      },
      {
        text: 'Videos',
        url: '#',
        current: false,
      },
      {
        text: 'Fans',
        url: '#',
        current: false,
      },
      {
        text: 'News',
        url: '#',
        current: false,
      },
      {
        text: 'Shop',
        url: '#',
        current: false,
      },
    ]
  }),
};
</script>

<template>
  <header>
    <nav class="container">
      <div>
        <a href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
      </div>
      <div>
        <ul>
          <li v-for="menuItem in menuItems" :key="menuItem.text"><a href="#">{{ menuItem.text }}</a></li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<style scoped>
nav {
  height: 70px;
  padding: 2rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

ul {
  list-style: none;
  display: flex;
  gap: 20px;
}

a {
  text-decoration: none;
  color: black;
  text-transform: uppercase;
  font-weight: bolder;
}

img {
  max-width: 100%;
  height: auto;
}

.container {
  width: 1200px;
  margin: 0 auto;
}
</style>
