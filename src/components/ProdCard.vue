<template>
	<div class="box-container">
		<div class="box">
			<img :src="details.thumb" :alt="details.series" />
		</div>
		<div class="text">{{ details.series }}</div>
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
.box-container {
	width: calc(100% / 6 - 20px);
	margin-right: 20px;
	margin-bottom: 50px;
	.box {
		height: 175px;
		overflow-y: hidden;
		cursor: pointer;
	}
	.text {
		color: white;
		font-size: 16px;
		margin-top: 20px;
		max-width: 190px;
		text-transform: uppercase;
	}
}
</style>
