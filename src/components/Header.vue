<template>
    <div class="header" id="header-wrap">
        <div class="container-fluid">
            <nav class="navbar navbar-expand-lg navbar-light " v-bind:class=" { 'navbarOpen': show }" @click.stop="toggleNavbar()">
                <a class="navbar-brand" href="#">
                    <img alt="Vue logo" src="../assets/images/logo.svg" />
                </a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation" @click.stop="toggleNavbar()">
                    <span class="hamburger"></span>
                     <span class="hamburger"></span>
                      <span class="hamburger"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent" v-bind:class="{ 'show': show }">
                    <ul class="navbar-nav">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Benefits</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Facilities</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Gallery</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Pricing</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact us</a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
        show: true
        }
    },
    mounted() {
		this.fixedHeader();
	},
    methods: {
		fixedHeader(){
			window.onscroll = function() {
				var header = document.getElementById("header-wrap");
				if (window.pageYOffset > 210) {
					 header.classList.add("dark-bg");
				} 
				else {
					 header.classList.remove("dark-bg");
				}
			}
		},
        toggleNavbar() {
            this.show = !this.show
        }
	}	
}
</script>
