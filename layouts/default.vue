<template>
	<div
		class="default-layout bg-slate-700 text-grey-400 min-h-screen justify-center items-center"
	>
		<p
			class="text-lg font-semibold text-white"
			style="font-size: 20px; border: 1px solid white"
		>
			Default layout
		</p>
		<hr style="margin-top: 10px; margin-bottom: 10px" />
		<slot />
	</div>
</template>

<script>
export default {
	setup() {
		return {};
	},
};
</script>

<style scoped>
.DefaultLayout {
	padding: 20px;
	min-height: 100vh;
}
</style>
