<template>
	<div id="app">
		<!-- HEADER -->
		<Header />
		<!-- CONTENT -->
		<Content />
		<!-- MAIN -->
		<Main />
		<!-- FOOTER -->
		<Footer />
	</div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
	name: "App",
	components: {
		Header,
		Content,
		Main,
		Footer,
	},
};
</script>

<style lang="scss">
@import "./scss/general.scss";
@import "./scss/utilities.scss";
</style>
