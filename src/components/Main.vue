<template>
	<main>
		<div class="container">
			<div class="column">
				<h1>DC Comics</h1>
				<ul class="dc-comics">
					<li>
						<a
							v-for="(link, index) in dcComics"
							:key="index"
							:href="link.url"
							>{{ link.text }}</a
						>
					</li>
				</ul>
				<h1>DC Comics</h1>
				<ul class="dc-comics">
					<li>
						<a v-for="(link, index) in shop" :key="index" :href="link.url">{{
							link.text
						}}</a>
					</li>
				</ul>
			</div>
			<div class="column">
				<h1>DC Comics</h1>
				<ul class="dc-comics">
					<li>
						<a v-for="(link, index) in dc" :key="index" :href="link.url">{{
							link.text
						}}</a>
					</li>
				</ul>
			</div>
			<div class="column">
				<h1>DC Comics</h1>
				<ul class="dc-comics">
					<li>
						<a v-for="(link, index) in sites" :key="index" :href="link.url">{{
							link.text
						}}</a>
					</li>
				</ul>
			</div>
			<!-- <img class="bg-logo" src="../assets/img/dc-logo-bg.png" alt="" /> -->
		</div>
	</main>
</template>

<script>
export default {
	name: "Main",
	data() {
		return {
			dcComics: [
				{ text: "Characters", url: "/characters", current: false },
				{ text: "Comics", url: "/comics", current: false },
				{ text: "Movies", url: "/movies", current: true },
				{ text: "Tv", url: "/tv", current: false },
				{ text: "Games", url: "/games", current: false },

				{ text: "Videos", url: "/videos", current: false },

				{ text: "News", url: "/news", current: false },
			],
			shop: [
				{ text: "Shop DC", url: "/Shop DC", current: false },
				{
					text: "Shop CD Collectibles",
					url: "/Shop CD Collectibles",
					current: false,
				},
			],
			dc: [
				{ text: "Terms Of Use", url: "/Terms Of Use", current: false },
				{
					text: "Privacy policy (New)",
					url: "/Privacy policy (New)",
					current: false,
				},
				{ text: "Ad Choices", url: "/Ad Choices", current: true },
				{ text: "Advertising", url: "/Advertising", current: false },
				{ text: "Jobs", url: "/Jobs", current: false },
				{ text: "Subscriptions", url: "/Subscriptions", current: false },
				{ text: "Talent Workshops", url: "/Talent Workshops", current: false },
				{
					text: "CPSC Certificates",
					url: "/CPSC Certificates",
					current: false,
				},
				{ text: "Ratings", url: "/Ratings", current: false },
				{ text: "Shop Help", url: "/Shop Help", current: false },
				{ text: "Contact Us", url: "/Contact Us", current: false },
			],
			sites: [
				{ text: "DC", url: "/DC", current: false },
				{ text: "MAD Magazine", url: "/MAD Magazine", current: false },
				{ text: "DC Kids", url: "/DC Kids", current: true },
				{ text: "DC Universe", url: "/DC Universe", current: false },
				{ text: "DC Power Visa", url: "/DC Power Visa", current: false },
			],
		};
	},
};
</script>

<style scoped>
main {
	background-image: url(../assets/img/footer-bg.jpg);
	background-position: center;
	background-repeat: no-repeat;
	background-size: cover;
	padding: 0px 10px;
}

.container {
	background-image: url(../assets/img/dc-logo-bg.png);
	background-position: right;
	background-repeat: no-repeat;
	background-size: 700px;
	margin: 0 auto;
	display: flex;
}

.column {
	min-width: 200px;
	margin: 40px 0px;
}

h1 {
	color: white;
	margin-bottom: 20px;
}
.dc-comics {
	list-style: none;
}

ul {
	display: flex;
	flex-direction: column;
	margin-bottom: 25px;
}

ul:nth-child(3) {
	margin-bottom: 0px;
}

li a {
	/* display: block; */
	display: flex;
	flex-direction: column;
	text-decoration: none;
	color: white;
	margin-bottom: 10px;
}

/* img.bg-logo {
	height: 700px;
	/* transform: translateY(-120px); */
/* overflow-y: hidden;
/* } */
</style>
