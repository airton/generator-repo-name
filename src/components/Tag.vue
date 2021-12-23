<template>
	<span 
		class="text-sm font-medium border py-1 px-2 rounded align-middle"
		v-bind:class="{[`border-${color}-500 text-${color}-500`]: color}" 
	>
		{{name}}
	</span>
</template>

<script>
export default {
	name: "Tag",
	props: ["name", "color"]
}
</script>