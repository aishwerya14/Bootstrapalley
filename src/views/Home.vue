<template>
  <div class="home">
    <Header></Header>
	<Banner></Banner>
	<Benefits></Benefits>
	<Facilities></Facilities>
	<Gallery></Gallery>
	<Pricing></Pricing>
	<Contact-us></Contact-us>
	<Map></Map>
	<Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Banner from "@/components/Banner.vue";
import Benefits from "@/components/Benefits.vue";
import Facilities from "@/components/Facilities.vue";
import Gallery from "@/components/Gallery.vue";
import ContactUs from "@/components/ContactUs.vue";
import Footer from "@/components/Footer.vue";
import Map from "@/components/Map.vue";
import Pricing from "@/components/Pricing.vue";


export default {
 	 name: "Home",
	components: {
			Header,
			Banner,
			Benefits,
			Facilities,
			Gallery,
			ContactUs,
			Map,
			Footer,
			Pricing
	}
};
</script>
