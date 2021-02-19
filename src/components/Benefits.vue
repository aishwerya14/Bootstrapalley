<template>
    <div class="benefits-wrap">
        <div class="container">
            <div class="title-sec">
                <h3>Benefits</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales...</p>
            </div>
            <div class="features-list">
                <div class="row">
                    <div 
                        v-for="item in features" :key="item"
                        class="col-sm-12 col-lg-4 feature">
                        <div class="icon-wrap">
                            <img alt="feature" :src="item.image" />
                            {{ item.name }} 
                        </div>
                        <div class="feature-content">
                            <h5> {{ item.heading }}</h5>
                            <p> {{ item.discription }}</p>
                        </div>
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
                features: [
                    {   
                        image: require("../assets/images/feature-1.svg") ,
                        heading: "Like Minded Startups", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                    {   
                        image: require("../assets/images/feature-2.svg" ),
                        heading: "Large Terrace", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                    {   
                        image: require("../assets/images/feature-3.svg") ,
                        heading: "Large Terrace", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                    {   
                        image: require("../assets/images/feature-4.svg") ,
                        heading: "Free Unlimited Wi-Fi", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                    {   
                        image: require("../assets/images/feature-5.svg") ,
                        heading: "Located on Main Road", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                    {   
                        image: require("../assets/images/feature-6.svg") ,
                        heading: "Hit the Target", 
                        discription:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales..."
                    },
                ]
        }
    }
}
</script>