<template>
	<div>
		<site-header />
		<div class="hero text-white">
			<intro />
		</div>
		<div class="hero-alt">
			<services/>
		</div>
		<div class="hero text-white">
			<clients />
		</div>
		<div class="hero-alt">
			<contact />
		</div>
	</div>
</template>

<script>
	import SiteHeader from "./Components/SiteHeader";
	import Intro from "./Components/Intro";
	import Services from "./Components/Services";
	import Clients from "./Components/Clients";
	import Contact from "./Components/Contact";

	export default {
		name: "App",
		components: { SiteHeader, Intro, Services, Clients, Contact }
	}
</script>