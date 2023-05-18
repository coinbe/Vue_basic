<template>
	<div>
		<h1>Parent</h1>
		<p>접속중인 {{ mySitename }} 사이트입니다</p>
		<br />
		<child :mySitename.sync="mySitename"></child>
	</div>
</template>

<script>
import Child from './Childe.vue';
export default {
	components: {
		Child,
	},
	data() {
		return {
			mySitename: 'naver.com',
		};
	},
};
</script>

<style></style>
