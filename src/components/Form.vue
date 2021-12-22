<template>
	<form class="mt-8 space-y-6" action="#" method="POST" @submit="onSubmit">
		<div class="flex items-center border-b border-teal-500 py-2">
			<div class="inline-block relative w-36 mr-1">
				<select v-model="startupName" @change="onChange" class="block appearance-none w-full bg-white border border-gray-400 hover:border-gray-500 px-4 py-2 pr-6 rounded shadow leading-tight focus:outline-none focus:shadow-outline">
					<option selected>iq</option>
					<option>azulis</option>
					<option>ccbr</option>
				</select>
				<div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
					<svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
				</div>
			</div>

			<input v-model="projectName" @input="onChange" class="appearance-none bg-transparent border-none w-full text-gray-700 mr-3 py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="digite aqui o nome" aria-label="Name"/>

			<div class="inline-block relative w-36 mr-1">
				<select v-model="projectType" @change="onChange" class="block appearance-none w-full bg-white border border-gray-400 hover:border-gray-500 px-4 py-2 pr-6 rounded shadow leading-tight focus:outline-none focus:shadow-outline">
					<option selected>ui</option>
					<option>app</option>
					<option>job</option>
					<option>api</option>
					<option>edge</option>
				</select>
				<div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
					<svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
				</div>
			</div>
		</div>
		<div class="flex items-center border-b border-green-500 py-2">
			<div class="col-span-3 sm:col-span-2 w-full">
				<label for="company-website" class="block text-sm font-medium text-green-500">
					Preview:
				</label>
				<div class="mt-1 flex w-full">
					<span class="block bg-white border border-green-400 px-2 py-2 rounded shadow shadow-red-500/40 md:shadow-green-500/40 leading-tight text-green-400">
						https://github.com/RedVentures/
					</span>
					<div class="flex items-center w-full text-green-500">
						<input class="appearance-none bg-transparent border-none w-full text-purple-500 font-bold py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="nome-projeto" aria-label="Project name" disabled v-model="result">
						<button type="submit">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 stroke-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 5H6a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2v-1M8 5a2 2 0 002 2h2a2 2 0 002-2M8 5a2 2 0 012-2h2a2 2 0 012 2m0 0h2a2 2 0 012 2v3m2 4H10m0 0l3-3m-3 3l3 3" />
							</svg>
						</button>
					</div>
				</div>
			</div>
		</div>
	</form>
</template>

<script>
import slugify from "/src/utils/slugify"

export default {
	nane: "Form",
	data() {
    return {
      startupName: "iq",
      projectType: "ui",
      projectName: "",
      result: ""
    }
  },
  methods: {
    onChange(e) {
      e.preventDefault()
      this.result = `${this.startupName}-${slugify(this.projectName)}-${this.projectType}`
    },
		onSubmit(e) {
			e.preventDefault()
			const formData = new FormData(document.querySelector("form"))
			const formProps = Object.fromEntries(formData)
			console.log(formProps)
			console.log(e)
		}
  }
}
</script>