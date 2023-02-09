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
			emitData2: '상위컴포넌트로 동신전달',
		};
	},
	methods: {
		sendParent() {
			this.$emit('send', this.emitData);
		},
		sendParent2() {
			this.$emit('send', this.emitData2);
		},
	},
};
</script>

<style></style>
