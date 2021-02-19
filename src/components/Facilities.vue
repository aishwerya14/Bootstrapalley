<template>
    <div class="facilities-wrap">
        <div class="container">
            <div class="title-sec">
                <h3>Facilities</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales...
                </p>
            </div>
            <div class="listwrap">
                <div class="row">
                    <div 
                        v-for="item in list" :key="item"   
                        class="col-sm-12 col-md-6 col-lg-3 list-item">
                        <div class="icon-wrap">
                            <img alt="feature" :src="item.image" />
                        </div>
                        <p>{{ item.title }} </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
     data() {
        return {
            list: [
                {   
                    image: require("../assets/images/icon1.svg") ,
                    title: "24/7 Access",
                },
                {   
                    image: require("../assets/images/icon2.svg") ,
                    title: "Spacious Cubicles",
                },
                {   
                    image: require("../assets/images/icon3.svg") ,
                    title: "24/7 Power Backup",
                },
                {   
                    image: require("../assets/images/icon4.svg") ,
                    title: "Printer Facilities",
                },

                {   
                    image: require("../assets/images/icon5.svg") ,
                    title: "CCTV & Access Cards",
                },
                {   
                    image: require("../assets/images/icon6.svg") ,
                    title: "Fridge & Microwave",
                },

                {   
                    image: require("../assets/images/icon7.svg") ,
                    title: "TV & Set Top Box",
                },

                {   
                    image: require("../assets/images/icon8.svg") ,
                    title: "Reception Area",
                },
                {   
                    image: require("../assets/images/icon9.svg") ,
                    title: "Large Cafeteria",
                },

                {   
                    image: require("../assets/images/icon10.svg") ,
                    title: "TV Conference Rooms",
                },
                {   
                    image: require("../assets/images/icon12.svg") ,
                    title: "Various Meeting Rooms",
                },
                {   
                    image: require("../assets/images/icon13.svg") ,
                    title: "Postal Address",
                },
                {   
                    image: require("../assets/images/icon14.svg") ,
                    title: "Large Open Terrace",
                },
                {   
                    image: require("../assets/images/icon1.svg") ,
                    title: "Housekeeping Facilities",
                },

                {   
                    image: require("../assets/images/icon1.svg") ,
                    title: "Parking Spaces",
                },
            ]
        }
     }
}
</script>
            