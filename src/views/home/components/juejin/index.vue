<template>
	<div class="juejin-view">
		<div class="container">掘金CSS艺术之美</div>
		<div>
			<button ref="red-theme-bt">切换红色主题</button>
			<button ref="blue-theme-bt">切换蓝色主题</button>
			<button ref="green-theme-bt">切换绿色主题</button>
		</div>
	</div>
</template>

<script>
import { defineComponent } from 'vue';
import './index.less';

export default defineComponent({
	name: 'juejin',
	data() {
		a: 1;
	},
	mounted() {
		debugger;
		console.log(this.a);
		console.log(1);
		[('red', 'blue', 'green')].forEach(v => {
			console.log('v: ', v);
			// const btn = document.getElementById(`${v}-theme-btn`);
			// console.log('btn: ', btn);
			// this.$refs[v].addEventListener('click', () => {
			// 	console.log('click: ');
			// 	document.body.style.setProperty('--bg-color', v);
			// });
		});
	},
});
</script>
