<template>
	<div class="flex flex-col min-h-screen">
		<AppHeader/>
		<main class="flex-grow">
			<slot/>
		</main>
		<AppFooter/>
		<ToastContainer/>
		<FloatingThemeToggle />
	</div>
</template>

<script setup lang="ts">
import ToastContainer from '~/components/common/ToastContainer.vue';
import AppHeader from '~/components/layout/AppHeader.vue';
import AppFooter from '~/components/layout/AppFooter.vue';
import FloatingThemeToggle from "~/components/FloatingThemeToggle.vue";
</script>