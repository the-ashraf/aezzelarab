<template>
	<div class="container mx-auto px-4 py-16">
		<h2 class="text-3xl mb-8 text-center sm:text-right">اهم العملاء</h2>
		<div class="flex flex-wrap justify-center sm:justify-start">
			<div v-for="client in clients" class="sm:w-1/4 px-2 mb-4">
				<div class="block h-24 sm:h-32 md:h-40 w-24 sm:w-32 md:w-40 rounded-full overflow-hidden border-2 focus:outline-none">
					<img class="h-full w-full object-cover" :src="client.url" :alt="client.name" :title="client.name">
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "Clients",
		data() {
			return {
				clients: [
					{name: 'Tomorrow للطاقة الشمسية', url: '../images/tomorrowsolar.png'},
					{name: 'باك تو ناتشر', url: '../images/backtonature.png'},
					{name: 'صندوق العاملين بمجموعة شركات القاهره للدواجن', url: '../images/cairopoultry.png'},
					{name: 'فرقة كود مصر الموسيقيه', url: '../images/codemasr.png'},
					{name: 'الشركة المصريه للمخبوزات', url: '../images/egyptianbakery.png'},
					{name: 'جريدة هرم مصر‎', url: '../images/harammisr.png'},
					{name: 'صندوق العاملين بالشركة الوطنية للاسكان', url: '../images/nch.png'},
					{name: 'تشريفه‎', url: '../images/tashreefa.png'},
				]
			}
		}
	}
</script>