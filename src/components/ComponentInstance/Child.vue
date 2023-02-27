<template>
	<div>
		<ul>
			<li>Component-Instance</li>
			<button @click="goParent()">VueJS</button>
		</ul>
	</div>
</template>

<script>
export default {
	data() {
		return {
			test: 'Hi',
		};
	},
	methods: {
		goParent() {
			this.$parent.goChild();
		},
		hiParent() {
			alert(this.test);
		},
	},
};
</script>

<style></style>
