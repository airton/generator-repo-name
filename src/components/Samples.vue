<template>
	<div class="py-10">
		<h3 class="flex block w-100 text-m font-bold text-gray-700 border-b border-teal-500 mb-5">
			Exemplos de Projetos
		</h3>
		<div class="mb-5">
			<p class="flex block w-100 text-sm text-green-500 mb-5">Billdesk:</p>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-billdesk-ui</span>
				<div class="ml-10"><Tag name="front end" color="pink" /></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-billdesk-app</span>
				<div class="ml-10"><Tag name="app mobile" color="purple" ></Tag></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-billdesk-api</span>
				<div class="ml-10"><Tag name="api" color="yellow" ></Tag></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-billdesk-edge</span>
				<div class="ml-10"><Tag name="lambda" color="blue" ></Tag></div>
			</div>
		</div>
		<div class="mb-5">
			<p class="flex block w-100 text-sm text-green-500 mb-5">Marketplace:</p>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-marketplace-ui</span>
				<div class="ml-10"><Tag name="front end" color="pink" /></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-marketplace-app</span>
				<div class="ml-10"><Tag name="app mobile" color="purple" ></Tag></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-marketplace-api</span>
				<div class="ml-10"><Tag name="api" color="yellow" ></Tag></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-marketplace-edge</span>
				<div class="ml-10"><Tag name="lambda" color="blue" ></Tag></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">iq-marketplace-job</span>
				<div class="ml-10"><Tag name="service" color="gray" ></Tag></div>
			</div>
		</div>
		<div class="mb-5">
			<p class="flex block w-100 text-sm text-green-500 mb-5">Azulis:</p>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">azulis-blog-ui</span>
				<div class="ml-10"><Tag name="front end" color="pink" /></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">azulis-landing-ui</span>
				<div class="ml-10"><Tag name="front end" color="pink" /></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">azulis-backoffice-ui</span>
				<div class="ml-10"><Tag name="front end" color="pink" /></div>
			</div>
			<div class="flex items-center mb-5">
				<span class="block text-center w-2/6 bg-white border border-gray-400 px-4 py-2 rounded shadow leading-tight">azulis-backoffice-api</span>
				<div class="ml-10"><Tag name="api" color="yellow" /></div>
			</div>
		</div>
	</div>
</template>

<script>
import Tag from "/src/components/Tag.vue"

export default {
	name: "Samples",
	components: {
		Tag
	}
}
</script>