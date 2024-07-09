<script setup>
import { useNuxtApp } from "#app";

const response = await $fetch("/api/hello");
console.log("response" + response);
const { $sayHelloPlugin } = useNuxtApp();
$sayHelloPlugin("world");
</script>
<template>
	<div
		class="min-h-screen text-white"
		style="margin-top: 10px; margin-bottom: 10px"
	>
		<Alert />
		<h1>Home (/)</h1>
		<Addition />
		<Color />
		<ContentDoc />
	</div>
</template>

<style lang="scss"></style>
