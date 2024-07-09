<script setup lang="ts">
import { useState } from "nuxt/app";

const counter = useState("counter", () => Math.round(Math.random() * 1000));
</script>

<template>
	<div class="text-white" style="margin-top: 10px; margin-bottom: 10px">
		Counter: {{ counter }}
		<button
			class="ml-1 p-1 border-2 border-slate-400 bg-slate-200 text-slate-800 text-sm rounded-lg shadow hover:bg-slate-300 focus:outline-none focus:ring-2 focus:ring-slate-400 active:bg-slate-400 transition ease-in-out duration-150"
			@click="counter++"
		>
			+
		</button>
		<button
			class="ml-1 p-1 border-2 border-slate-400 bg-slate-200 text-slate-800 text-sm rounded-lg shadow hover:bg-slate-300 focus:outline-none focus:ring-2 focus:ring-slate-400 active:bg-slate-400 transition ease-in-out duration-150"
			@click="counter--"
		>
			-
		</button>
	</div>
</template>
