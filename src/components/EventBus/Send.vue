<template>
	<div>
		<h1>Send</h1>
		<input v-model="text" />
		<button @click="send">보내기</button>
		<div v-if="receiveText">Send.vue : I sent a message</div>
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
			receiveText: '',
		};
	},
	methods: {
		send() {
			EventBus.$emit('message', this.text);
			this.text = '';
		},
		onReceive(text) {
			this.receiveText = text;
			console.log(this.receiveText);
		},
	},
};
</script>

<style></style>
