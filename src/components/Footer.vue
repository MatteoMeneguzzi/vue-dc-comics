<template>
	<footer>
		<div class="container">
			<button class="sign-up">sign-up now!</button>
			<ul class="socials">
				<li class="social">
					<a href="">follow us</a>
				</li>
				<li class="social">
					<a href=""
						><img src="../assets/img/footer-facebook.png" alt="Facebook"
					/></a>
				</li>
				<li class="social">
					<a href=""
						><img src="../assets/img/footer-twitter.png" alt="twitter"
					/></a>
				</li>
				<li class="social">
					<a href=""
						><img src="../assets/img/footer-youtube.png" alt="youtube"
					/></a>
				</li>
				<li class="social">
					<a href=""
						><img src="../assets/img/footer-pinterest.png" alt="pinterest"
					/></a>
				</li>
				<li class="social">
					<a href=""
						><img src="../assets/img/footer-periscope.png" alt="periscope"
					/></a>
				</li>
			</ul>
		</div>
	</footer>
</template>

<script>
export default {
	name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../scss/vars";

footer {
	background: #303030;
	padding: 20px 0px;
}
.container {
	display: flex;
	justify-content: space-between;
	padding: 10px;
	.sign-up {
		border: 2px solid $primary-blue;
		padding: 10px;
		font-size: 20px;
		text-transform: uppercase;
		background: #303030;
		color: #fff;
		cursor: pointer;
	}
	ul {
		display: flex;
		align-items: center;
		list-style: none;
		li {
			a {
				text-decoration: none;
				margin-left: 10px;
				color: $primary-blue;
				text-transform: uppercase;
				font-weight: bold;
			}
		}
	}
}
</style>
