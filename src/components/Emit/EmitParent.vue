<template>
	<div>
		<h1>Parent Component</h1>
		<EmitChild @send="changeText" />
	</div>
</template>

<script>
import EmitChild from '@/components/Emit/EmitChild.vue';
export default {
	components: {
		EmitChild,
	},
	data() {
		return {
			text: '',
		};
	},
	methods: {
		changeText(emitData) {
			console.log(emitData);
			this.text = emitData;
		},
	},
};
</script>

<style></style>
