<template>
	<div class="about-view">
		<img
			v-show="tab === 0"
			class="about-qrcode"
			src="https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/03bcc13d83524f9eb8a61a1cab0543af~tplv-k3u1fbpfcp-watermark.image"
		/>
		<img
			v-show="tab === 1"
			class="about-qrcode"
			src="https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/f9a7e606f0ca4cf58c2262f6c16e3464~tplv-k3u1fbpfcp-watermark.image"
		/>
		<button class="about-btn center" @click="setTab">
			查看{{ tab === 0 ? '公众号' : '微信' }}
		</button>
	</div>
</template>

<script>
import { defineComponent, ref } from 'vue';
import style from './index.less';

export default defineComponent({
	name: 'about',
	setup() {
		const tab = ref(0);
		const setTab = () => (tab.value = tab.value === 0 ? 1 : 0);
		return { setTab, tab };
	},
});
</script>
