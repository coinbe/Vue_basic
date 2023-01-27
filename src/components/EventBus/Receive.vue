<template>
	<div>
		<h1>Receive</h1>
		<div v-if="text">Receive.vue</div>
	</div>
</template>

<script>
import EventBus from './EventBus';

export default {
	created() {
		EventBus.$on('message', this.onReceive);
	},
	data() {
		return {
			text: '',
		};
	},
	methods: {
		onReceive(text) {
			this.text = text;
		},
	},
};
</script>

<style></style>
