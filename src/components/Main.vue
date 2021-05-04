<template>
    <main>
        <div class="column">
            <ul class="dc-comics" >
                <li>
                    <a v-for="(link,index) in dcComics" :key="index" :href="link.url">{{link.text}}</a>
                </li>
            </ul>
            <ul class="dc-comics" >
                <li>
                    <a v-for="(link,index) in dcComics" :key="index" :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </div>
        <div class="column"></div>
        <div class="column"></div>
    </main>
</template>

<script>
export default {
    name: "Main",
    data() {
        return {
            dcComics: [
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
            ],
            shop: [
                { text: "Shop DC", url: '/Shop DC', current: false},
                { text: "Shop CD Collectibles", url: '/Shop CD Collectibles', current: false},
            ],
            dc: [
                { text: "Terms Of Use", url: '/Terms Of Use', current: false},
                { text: "Privacy policy (New)", url: '/Privacy policy (New)', current: false},
                { text: "Ad Choices", url: '/Ad Choices', current: true},
                { text: "Advertising", url: '/Advertising', current: false},
                { text: "Jobs", url: '/Jobs', current: false},
                { text: "Subscriptions", url: '/Subscriptions', current: false},
                { text: "Talent Workshops", url: '/Talent Workshops', current: false},
                { text: "CPSC Certificates", url: '/CPSC Certificates', current: false},
                { text: "Ratings", url: '/Ratings', current: false},
                { text: "Shop Help", url: '/Shop Help', current: false},
                { text: "Contact Us", url: '/Contact Us', current: false}
            ],
            sites: [
                { text: "DC", url: '/DC', current: false},
                { text: "MAD Magazine", url: '/MAD Magazine', current: false},
                { text: "DC Kids", url: '/DC Kids', current: true},
                { text: "DC Universe", url: '/DC Universe', current: false},
                { text: "DC Power Visa", url: '/DC Power Visa', current: false},
            ]
        }
    }
}
</script>

<style scoped>
    main {
        background-image: url(../assets/img/footer-bg.jpg);
        height: 500px;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        padding: 40px 0px;
    }
    .column {
        height: 500px;
        display: flex;
        flex-direction: column;
    }
    .dc-comics {
        list-style: none;
        display: flex;
        flex-direction: column;
    }
    li a {
        display: block;
        text-decoration: none;
        color: white;
    }
</style>