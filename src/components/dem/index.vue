<template>
	<div className="dem-component">Dem Component {{done}}</div>
</template>

<style lang="scss">
.dem-component {
	font-size: 20px;
	color: #f66;
}
</style>

<script>
import { defineComponent } from "vue";

export default defineComponent({
	name: "dem",
	props: {
		done: {
			default: "Done",
			type: String
		}
	}
});
</script>