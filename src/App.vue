<template>
	<div id="app">
		<!-- <Ref /> -->
		<Receive />
		<Send />
	</div>
</template>

<script>
// import Ref from '@/components/Ref/Ref.vue';
import Receive from '@/components/EventBus/Receive.vue';
import Send from '@/components/EventBus/Send.vue';
export default {
	name: 'App',
	components: {
		// Ref,
		Receive,
		Send,
	},
};
</script>

<style></style>
