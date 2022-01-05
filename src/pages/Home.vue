<template>
	<div class="min-h-full flex items-center justify-center py-12 px-4 sm:px-6 lg:px-8">
		<div class="max-w-2xl w-full space-y-8">
			<Header />
			<Form />
			<Types />
			<Samples />
			<GoodPractices />
      <div class="flex items-center justify-center border-t border-teal-500 pt-5">
        <p class="text-center text-gray-600">Made by iq tech team ❤️</p>
      </div>
		</div>
  </div>
</template>

<script>
import Header from "/src/components/Header.vue"
import Form from "/src/components/Form.vue"
import Types from "/src/components/Types.vue"
import Samples from "/src/components/Samples.vue"
import GoodPractices from "/src/components/GoodPractices.vue"

export default {
  name: "Home",
  components: {
    Header,
    Form,
    Types,
    Samples,
    GoodPractices
  }
}
</script>