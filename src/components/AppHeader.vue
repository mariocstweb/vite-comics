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

<style lang="scss" scoped>
// @use "../assets/style.scss" as *;

nav {
  min-height: 70px;
  padding: 0.8rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-shrink: 0;
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
  font-size: 12px;
}

img {
  max-width: 100%;
  height: auto;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
