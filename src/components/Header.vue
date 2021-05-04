<template>
  <header>
      <a href="">
          <img src="../assets/img/dc-logo.png" alt="logo-dc">
      </a>

      <nav>
          <ul>
              <li v-for="(link, index) in links" :key="index" >
                  <a :class="{ active: link.current}" :href="link.url">{{link.text}}</a>
              </li>
              
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return {
            links: [
                { text: "characters", url: '/characters', current: false},
                { text: "comics", url: '/comics', current: false},
                { text: "movies", url: '/movies', current: true},
                { text: "tv", url: '/tv', current: false},
                { text: "games", url: '/games', current: false},
                { text: "collectibles", url: '/collectibles', current: false},
                { text: "videos", url: '/videos', current: false},
                { text: "fans", url: '/fans', current: false},
                { text: "news", url: '/news', current: false},
                { text: "shop", url: '/shop', current: false}
            ]
        }
    }
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 150px;
        padding: 0px 10px;
        max-width: 1070px;
        margin: 0 auto;
    }

    header nav { 
        text-transform: uppercase;
    }
    ul {
        display: flex;
        list-style: none;
    }
    li a {
        text-decoration: none;
        margin-left: 10px;
        color: black;
        padding: 56px 0px;
        font-weight: bold;
    }
    li a:hover,
    li a.active {
        color: #427cec;
        border-bottom: 8px solid #427cec;
    }

</style>