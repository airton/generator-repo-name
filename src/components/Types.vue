<template>
	<div class="py-10">
		<h3 class="flex block w-100 text-m font-bold text-gray-700 border-b border-teal-500 mb-10">
			Tipos
		</h3>
		<div class="flex items-center mb-5">
			<span class="block text-center w-1/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">ui</span>
			<p class="px-4 py-2 w-5/6">
				Esse seria usado para projetos contendo o 
				<Tag name="front end" color="pink" />
				da aplicação, a parte visual onde o usuário interage.
			</p>
		</div>
		<div class="flex items-center mb-5">
			<span class="block text-center w-1/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">app</span>
			<p class="px-4 py-2 w-5/6">
				Esse seria usado para projetos contendo o 
				<Tag name="app mobile" color="purple" ></Tag> 
				da aplicação, onde o usuário instala no seu celular o aplicativo.
			</p>
		</div>
		<div class="flex items-center mb-5">
			<span class="block text-center w-1/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">api</span>
			<p class="px-4 py-2 w-5/6">
				Esse seria usado para projetos contendo a 
				<Tag name="api" color="yellow" ></Tag> 
				da aplicação, e o front end fara o usuo dela.
			</p>
		</div>
		<div class="flex items-center mb-5">
			<span class="block text-center w-1/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">job</span>
			<p class="px-4 py-2 w-5/6">
				Esse seria usado para projetos contendo algum 
				<Tag name="service" color="gray" ></Tag>, 
				que fazem integração com parceiros...
			</p>
		</div>
		<div class="flex items-center mb-5">
			<span class="block text-center w-1/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">edge</span>
			<p class="px-4 py-2 w-5/6">
				Esse seria usado para projetos contendo 
				<Tag name="lambda" color="blue" ></Tag>. 
			</p>
		</div>
	</div>
</template>

<script>
import Tag from "/src/components/Tag.vue"

export default {
	name: "Types",
	components: {
		Tag
	}
}
</script>