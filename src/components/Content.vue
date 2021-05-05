<template>
	<section>
		<div class="jumbotron-background"></div>
		<div class="black-area">
			<div class="container">
				<ProdCard
					v-for="(product, index) in products"
					:key="index"
					:details="product"
				/>
				<a href=""><button class="load-more">Load more</button></a>
			</div>
		</div>
		<div class="blu-area">
			<div class="container">
				<ul class="services">
					<!-- <li v-for="(link, index) in links" :key="index">
						<img :src="`../assets/img/buy${link.img}`" :alt="link.text" />
						<a :class="{ active: link.current }" :href="link.url">{{
							link.text
						}}</a>
					</li> -->
					<li class="service">
						<img
							src="../assets/img/buy-comics-digital-comics.png"
							alt="digital-comics"
						/>
						<a href="">DIGITAL COMICS</a>
					</li>
					<li class="service">
						<img
							src="../assets/img/buy-comics-merchandise.png"
							alt="merchandise"
						/>
						<a href="">DIGITAL COMICS</a>
					</li>
					<li class="service">
						<img
							src="../assets/img/buy-comics-subscriptions.png"
							alt="subscriptions"
						/>
						<a href="">DIGITAL COMICS</a>
					</li>
					<li class="service">
						<img
							src="../assets/img/buy-comics-shop-locator.png"
							alt="shop-locator"
						/>
						<a href="">DIGITAL COMICS</a>
					</li>
					<li class="service">
						<img
							src="../assets/img/buy-dc-power-visa.svg"
							alt="dc-power-visa"
						/>
						<a href="">DIGITAL COMICS</a>
					</li>
				</ul>
			</div>
		</div>
	</section>
</template>

<script>
import ProdCard from "@/components/ProdCard.vue";
export default {
	name: "Content",
	components: {
		ProdCard,
	},
	data() {
		return {
			links: [
				{
					text: "digital comics",
					url: "/digital comics",
					img: "-comics-digital-comics.png",
				},
				{
					text: "dc merchandise",
					url: "/dc merchandise",
					img: "-comics-merchandise.png",
				},
				{
					text: "subscription",
					url: "/subscription",
					img: "-comics-subscriptions.png",
				},
				{
					text: "comic shop locator",
					url: "/comic shop locator",
					img: "-comics-shop-locator.png",
				},
				{
					text: "dc power visa",
					url: "/dc power visa",
					img: "-dc-power-visa.svg",
				},
			],
			products: [
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
					price: "$19.99",
					series: "Action Comics",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
					price: "$3.99",
					series: "American Vampire 1976",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
					price: "$16.99",
					series: "Aquaman",
					type: "graphic novel",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
					price: "$2.99",
					series: "Batgirl",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
					price: "$3.99",
					series: "Batman",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
					price: "$2.99",
					series: "Batman Beyond",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
					price: "$3.99",
					series: "Batman/Superman",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
					price: "$4.99",
					series: "Batman/Superman Annual",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
					price: "$5.99",
					series: "Batman: The Joker War Zone",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
					price: "$6.99",
					series: "Batman: Three Jokers",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
					price: "$4.99",
					series: "Batman: White Knight Presents: Harley Quinn",
					type: "comic book",
				},
				{
					thumb:
						"https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
					price: "$16.99",
					series: "Catwoman",
					type: "graphic novel",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../scss/vars";

.jumbotron-background {
	background-image: url(../assets/img/jumbotron.jpg);
	object-fit: cover;
	background-position: center top;
	background-repeat: no-repeat;

	height: 400px;
}

.black-area {
	background: black;
	color: #fff;
	padding: 0px 10px;
	font-size: 30px;
}

.black-area {
	.container {
		position: relative;

		display: flex;
		flex-wrap: wrap;
		padding: 100px 20px 0px;
		&::before {
			content: "current series";
			position: absolute;
			top: -40px;
			left: 0;
			padding: 20px 35px;
			background-color: $primary-blue;
			color: white;
			text-transform: uppercase;
			border: none;
			font-weight: bold;
		}
		a {
			text-decoration: none;
			margin: 0 auto;
			margin-bottom: 30px;

			button {
				padding: 20px 75px;
				background-color: $primary-blue;
				color: white;
				text-transform: uppercase;
				border: none;
				font-weight: bold;
				cursor: pointer;
			}
		}
	}
}

.blu-area {
	background: $primary-blue;
	color: #fff;
	padding: 40px 0px;
	text-transform: uppercase;
}
ul {
	min-width: 1000px;
	display: flex;
	list-style: none;
	justify-content: space-between;
	padding-right: 20px;
}
li {
	width: calc(100% / 5);
	display: flex;
	align-items: center;
	padding: 0px 40px;
}

li img {
	max-width: 100%;
	max-height: 50%;
}

li:last-child img {
	max-height: 30%;
}

li.service a {
	display: inline-block;
	min-width: 150px;
	text-decoration: none;
	color: white;
	font-size: 14px;
	margin-left: 15px;
}
</style>
