<template>
	<div>
		<p>Child</p>
		<p>{{ text }}</p>
		<button @click="changeText">Extends ChangeText</button>
	</div>
</template>

<script>
import Parent from '@/components/Extends/Parent.vue';
export default {
	extends: {
		Parent,
	},
	data() {
		return {
			count: 0,
			text: '',
		};
	},
	methods: {
		addCount() {
			this.count = this.count + 1;
		},
	},
};
</script>

<style></style>
