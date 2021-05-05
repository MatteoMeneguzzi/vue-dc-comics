<template>
	<div class="box">
		<img :src="details.thumb" :alt="details.series" />
		ciao
	</div>
</template>

<script>
export default {
	name: "Products",
	props: ["details"],
	// props: {
	//     details: Object
	// },
};
</script>

<style scoped lang="scss">
.box {
	width: calc((100% / 6) -);
	overflow-y: hidden;
	margin-bottom: 50px;

	img {
		// width: 100px;
	}
}
</style>
