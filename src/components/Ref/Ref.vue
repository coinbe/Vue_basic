<template>
	<div>
		안녕하세요
		<ref-person ref="RefPerson" name="dorosy" />
	</div>
</template>

<script>
import RefPerson from './RefPerson.vue';
export default {
	components: {
		RefPerson,
	},
	computed: {
		isExist() {
			// 랜더링 여부 검사
			console.log('isExist', this.$refs);
			return this.$refs.RefPerson ? true : false;
		},
	},
	created() {
		console.log('created : ', this.isExist);
	},
	mounted() {
		console.log('mounted : ', this.isExist);
		const name = this.$refs.RefPerson.name;
		console.log(name);

		this.$refs.RefPerson.sayHi();
	},
};
</script>

<style></style>
