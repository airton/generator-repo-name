<template>
	<span 
		class="text-sm font-medium border py-1 px-2 rounded align-middle"
		:class="classActive"
	>
		{{name}}
	</span>
</template>

<script>
export default {
	name: "Tag",
	props: ["name", "color"],
	data() {
		return {
			classActive: {
				'border-pink-500 text-pink-500': this.color === 'pink',
				'border-purple-500 text-purple-500': this.color == 'purple',
				'border-yellow-500 text-yellow-500': this.color == 'yellow',
				'border-gray-500 text-gray-500': this.color == 'gray',
				'border-blue-500 text-blue-500': this.color == 'blue',
			}
		}
	}
}
</script>