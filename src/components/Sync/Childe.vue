<template>
	<div>
		<h1>Child</h1>
		<p>{{ mySitename }}</p>
		<br />
		<br />
		<button @click="updateName">[바꾸기]</button>
	</div>
</template>

<script>
export default {
	props: {
		mySitename: String,
	},
	methods: {
		updateName() {
			// emit할때는 update:propName 형태로 만들어줘야한다
			this.$emit('update:mySitename', '');
		},
	},
};
</script>

<style></style>
