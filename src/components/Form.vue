<template>
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

		<!-- Show tooltip on top -->
		<!-- <button data-tooltip-target="tooltip-top" data-tooltip-placement="top" type="button" class="mb-2 md:mb-0 text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Tooltip top</button>
		<div id="tooltip-top" role="tooltip" class="inline-block absolute z-10 py-2 px-3 text-sm font-medium text-white bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
			Tooltip on top
			<div class="tooltip-arrow" data-popper-arrow></div>
		</div> -->

		<div class="flex items-center border-b border-green-500 py-2">
			<div class="col-span-3 sm:col-span-2 w-full">
				<label for="company-website" class="block text-sm font-medium text-green-500">
					Preview:
				</label>
				<div class="mt-1 flex w-full">
					<span class="flex items-center bg-white border border-green-400 px-2 py-2 rounded shadow shadow-green-500/40 md:shadow-green-500/40 leading-tight text-green-400">
						
					<!-- <svg width="24px" height="24px" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-green mr-1">
						<rect width="24" height="24" fill="white" fill-opacity="0.01"/>
						<path fill-rule="evenodd" clip-rule="evenodd" d="M24 4C12.9543 4 4 12.9543 4 24C4 35.0457 12.9543 44 24 44C35.0457 44 44 35.0457 44 24C44 12.9543 35.0457 4 24 4ZM0 24C0 10.7452 10.7452 0 24 0C37.2548 0 48 10.7452 48 24C48 37.2548 37.2548 48 24 48C10.7452 48 0 37.2548 0 24Z" fill="currentColor"/>
						<path fill-rule="evenodd" clip-rule="evenodd" d="M19.183 45.4715C18.9896 45.2218 18.9896 42.9972 19.183 38.798C17.1112 38.8695 15.8022 38.7257 15.256 38.3666C14.4368 37.8279 13.6166 36.1666 12.8889 34.9958C12.1612 33.825 10.546 33.6399 9.8938 33.3782C9.24158 33.1164 9.07785 32.0495 11.691 32.8564C14.3042 33.6633 14.4316 35.8606 15.256 36.3744C16.0804 36.8882 18.0512 36.6634 18.9446 36.2518C19.8379 35.8402 19.7722 34.3077 19.9315 33.7006C20.1329 33.1339 19.423 33.0082 19.4074 33.0036C18.5353 33.0036 13.9537 32.0072 12.6952 27.5705C11.4368 23.1339 13.0579 20.234 13.9227 18.9874C14.4992 18.1563 14.4482 16.3851 13.7697 13.6736C16.2333 13.3588 18.1344 14.1342 19.4732 16C19.4745 16.0107 21.2283 14.9571 24 14.9571C26.7718 14.9571 27.7551 15.8153 28.514 16C29.2728 16.1847 29.8798 12.734 34.5666 13.6736C33.5881 15.5968 32.7686 18 33.3941 18.9874C34.0195 19.9748 36.4742 23.1146 34.9664 27.5705C33.9611 30.5412 31.9851 32.3522 29.0382 33.0036C28.7002 33.1114 28.5313 33.2854 28.5313 33.5254C28.5313 33.8855 28.9881 33.9248 29.6463 35.6116C30.085 36.7361 30.1167 39.9479 29.7413 45.2469C28.7904 45.489 28.0506 45.6515 27.5219 45.7346C26.5845 45.8819 25.5667 45.9645 24.5666 45.9964C23.5666 46.0283 23.2193 46.0247 21.8368 45.896C20.9151 45.8102 20.0305 45.6687 19.183 45.4715Z" fill="currentColor"/>
					</svg> -->
						https://github.com/RedVentures/
					</span>
					<div class="flex items-center w-full text-green-500">
						<input id="project-name" class="appearance-none bg-transparent border-none w-full text-purple-500 font-bold py-1 px-2 leading-tight focus:outline-none" type="text" placeholder="nome-projeto" aria-label="Project name" disabled v-model="result">
						<button type="submit" @click="onClickCopy" class="block bg-white border border-green-400 px-2 py-2 rounded shadow shadow-green-500/40 md:shadow-green-500/40 leading-tight text-green-400">
							<svg v-if="loading" class="animate-spin h-6 w-6 text-green" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
								<circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
								<path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
							</svg>
							<svg v-else-if="!loading" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 stroke-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
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
      result: "",
			loading: false
    }
  },
  methods: {
    onChange(e) {
      e.preventDefault()
      this.result = `${this.startupName}-${slugify(this.projectName)}-${this.projectType}`
    },
		async onClickCopy(e) {
			e.preventDefault()
			this.loading = true

			await navigator.clipboard.writeText(this.result)

			setTimeout(() => {
				this.loading = false
			}, 1000)
		}
  }
}
</script>