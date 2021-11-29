<template>
	<div class="min-h-full flex items-center justify-center py-12 px-4 sm:px-6 lg:px-8">
		<div class="max-w-md w-full space-y-8">
			<div>
        <img class="mx-auto h-12 w-auto" src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg" alt="Workflow">
        <h2 class="mt-6 text-center text-3xl font-extrabold text-gray-900">
          Generetor Repo Name
        </h2>
        <!-- <p class="mt-2 text-center text-sm text-gray-600">
          Or
          <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500">
          start your 14-day free trial
          </a>
        </p> -->
			</div>
			<form class="mt-8 space-y-6" action="#" method="POST">
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
          <div class="inline-block relative w-36 mr-1">
            <select v-model="projectType" @change="onChange" class="block appearance-none w-full bg-white border border-gray-400 hover:border-gray-500 px-4 py-2 pr-6 rounded shadow leading-tight focus:outline-none focus:shadow-outline">
              <option selected>www</option>
              <option>app</option>
              <option>admin</option>
            </select>
            <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
              <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
            </div>
          </div>

          <input v-model="projectName" @input="onChange" class="appearance-none bg-transparent border-none w-full text-gray-700 mr-3 py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="digite aqui o nome" aria-label="Name">
        </div>
        <div class="flex items-center border-b border-teal-500 py-2">
          <div class="col-span-3 sm:col-span-2">
            <label for="company-website" class="block text-sm font-medium text-gray-700">
              Preview: {{startupName}}-{{projectType}}-{{projectName}}
            </label>
            <div class="mt-1 flex">
              <span class="block w-full bg-white border border-gray-400 px-4 py-2 pr-6 rounded shadow leading-tight text-gray-400">
                https://github.com/RedVentures/
              </span>
              <input class="appearance-none bg-transparent border-none w-full text-gray-700 mr-3 py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="nome-projeto" aria-label="Project name" v-model="result">
            </div>
          </div>
        </div>
			</form>
		</div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      startupName: "iq",
      projectType: "www",
      projectName: "",
      result: ""
    }
  },
  methods: {
    onChange(e) {
      e.preventDefault()
      this.result = `${this.startupName}-${this.projectType}-${this.projectName}`
    }
  }
}
</script>