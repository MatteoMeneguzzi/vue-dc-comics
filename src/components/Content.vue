<template>
  <section>
      <div class="black-area">
        <div class="container">ciao</div>
      </div>
      <div class="blu-area">
          <div class="container">
              <ul>
                  <li v-for="(link, index) in links" :key="index" >
                      <img :src="`../assets/img/buy${link.img}`" :alt="link.text">
                      <a :class="{ active: link.current}" :href="link.url">{{link.text}}</a>
                  </li>
              
              </ul>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Content",
    data() {
        return {
            links: [
                { text: "digital comics", url: '/digital comics', img: "-comics-digital-comics.png"},
                { text: "dc merchandise", url: '/dc merchandise', img: "-comics-merchandise.png"},
                { text: "subscription", url: '/subscription', img: "-comics-subscriptions.png"},
                { text: "comic shop locator", url: '/comic shop locator', img: "-comics-shop-locator.png"},
                { text: "dc power visa", url: '/dc power visa', img: "-dc-power-visa.svg"},  
            ]
        }
    }
}
</script>

<style scoped>
    

    .black-area {
        background: black;
        color: #fff;
         padding: 0px 10px;
         font-size: 30px;
        
    }

    .container {
        max-width: 1070px;
        margin: 0 auto;
    }
     .blu-area {
        background: #427cec;
        color: #fff;
        padding: 0px 10px;
        text-transform: uppercase;
        
    }
    ul {
        width: 100%;
        display: flex;
        list-style: none;
         justify-content: space-between;
    }

    li a {
        text-decoration: none;
        
        color: white;
        
    }
  

</style>