<template>
	<div class="py-10">
		<h3 class="flex block w-100 text-m font-bold text-gray-700 border-b border-teal-500 mb-5">
			Boas Práticas
		</h3>
		<div class="mb-5">
			<ol class="list-decimal list-inside">
				<li class="text-sm text-gray-500 mb-3">Usar nomes em inglês:
					<ul class="list-disc list-inside ml-10 mt-2">
						<li class="text-sm text-gray-500 mb-3">oque não fazer: 
							<span class="bg-white border border-red-600 px-1 py-1 rounded text-red-600">
								iq-parceiros-forms-ui
							</span>
						</li>
						<li class="text-sm text-gray-500 mb-3">oque fazer: 
							<span class="bg-white border border-green-600 px-1 py-1 rounded text-green-600">
								iq-partner-forms-ui
							</span>
						</li>
					</ul>
				</li>
				<li class="text-sm text-gray-500 mb-3">Evitar nomes abreviados:
					<ul class="list-disc list-inside ml-10 mt-2">
						<li class="text-sm text-gray-500 mb-3">oque não fazer: 
							<span class="bg-white border border-red-600 px-1 py-1 rounded text-red-600">
								iq-part-lp-ui
							</span>
						</li>
						<li class="text-sm text-gray-500 mb-3">oque fazer: 
							<span class="bg-white border border-green-600 px-1 py-1 rounded text-green-600">
								iq-partners-landingpage-ui
							</span>
						</li>
					</ul>
				</li>
				<li class="text-sm text-gray-500 mb-3">Evitar nomes muito longos:
					<ul class="list-disc list-inside ml-10 mt-2">
						<li class="text-sm text-gray-500 mb-3">oque não fazer: 
							<span class="bg-white border border-red-600 px-1 py-1 rounded text-red-600">
								iq-backoffice-integrations-utils-full-rest-api
							</span>
						</li>
						<li class="text-sm text-gray-500 mb-3">oque fazer: 
							<span class="bg-white border border-green-600 px-1 py-1 rounded text-green-600">
								iq-backoffice-integrations-api
							</span>
						</li>
					</ul>
				</li>
				<li class="text-sm text-gray-500 mb-3">Evitar números:
					<ul class="list-disc list-inside ml-10 mt-2">
						<li class="text-sm text-gray-500 mb-3">oque não fazer: 
							<span class="bg-white border border-red-600 px-1 py-1 rounded text-red-600">
								azulis-blog-v2-ui
							</span>
						</li>
						<li class="text-sm text-gray-500 mb-3">oque fazer: 
							<span class="bg-white border border-green-600 px-1 py-1 rounded text-green-600">
								azulis-blogger-ui
							</span>
						</li>
					</ul>
				</li>
			</ol>
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