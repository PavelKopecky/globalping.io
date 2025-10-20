<template>
	<section class="w-full flex flex-col items-center justify-center gap-4 min-h-screen relative duration-200 ease-in-out" :class="{'bg-black/90': switchColor}">
		<h3 class="font-bold text-3xl select-none duration-300" :class="{'text-blue-50': switchColor, 'text-blue-950': !switchColor}">Welcome to <span @click="switchColor = !switchColor" class="cursor-pointer bg-gradient-to-r from-green-400 to-blue-500 bg-clip-text text-transparent">Nuxt</span> pages!</h3>
		<small class="hidden">This page uses tailwindcss, if you see this message, it is not working properly.</small>
	</section>
</template>

<script setup lang="ts">
	const switchColor = ref(false);
</script>
