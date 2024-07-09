<script setup lang="ts">
import { useState } from "nuxt/app";

const useColor = () => useState<string>("color", () => "PINK");
const color = useColor();
</script>

<template>
	<div class="text-white" style="margin-top: 10px; margin-bottom: 10px">
		<p>
			Current color: <b> {{ color }}</b>
		</p>
	</div>
</template>
