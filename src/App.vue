<template>
	<div id="app">
		<!-- <Ref /> -->
		<!-- <Receive /> -->
		<!-- <Send /> -->
		<Parent />
		<!-- <EmitParent /> -->
	</div>
</template>

<script>
// import Ref from '@/components/Ref/Ref.vue';
// import Receive from '@/components/EventBus/Receive.vue';
// import Send from '@/components/EventBus/Send.vue';
// import EmitParent from '@/components/Emit/EmitParent.vue';
import Parent from '@/components/Sync/Parent.vue';
export default {
	name: 'App',
	components: {
		// Ref,
		// Receive,
		// Send,
		// EmitParent,
		Parent,
	},
};
</script>

<style></style>
