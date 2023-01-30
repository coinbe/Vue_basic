<template>
	<div>
		<h1>Child Component</h1>
		<button @click="sendParent">SEND</button>
	</div>
</template>

<script>
export default {
	data() {
		return {
			emitData: '상위컴포넌트로 전달',
		};
	},
	methods: {
		sendParent() {
			this.$emit('send', this.emitData);
		},
	},
};
</script>

<style></style>
