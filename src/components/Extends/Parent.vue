<template>
	<div>
		<h2>Parent</h2>
		<p>{{ text }}</p>
		<button @click="changeText">button</button>
	</div>
</template>

<script>
export default {
	data() {
		return {
			text: 'hello',
		};
	},
	methods: {
		changeText() {
			this.text = 'changeText';
		},
	},
};
</script>

<style></style>
