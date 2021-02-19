<template>
    <div class="gallery-wrap">
        <div class="container-fluid">
            <div class="title-sec">
                <h3>Gallery</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porta fringilla ullamcorper. Morbi felis orci, lacinia a velit et, sodales...</p>
            </div>
            <div class="img-wrap">
                <ul>
                    <li class="content" v-for="item in gallery" :key="item" :style="{'background-image': 'url(' + require('../assets/images/' + item.image) + ')'}">       
                        <div class="">
                            <a href="javascript:void(0)">
                            <div class="content-overlay"></div>
                            <!-- <img alt="gallery" :src="item.image" width="483" height="289"/>  -->
                            <div class="content-details fadeIn-top">
                                <h3>Gallery by Lorem</h3>
                                <p>Lorem Ispum asksn kjwdaubh</p>
                            </div>
                            </a>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
     data() {
        return {
            gallery: [
                {   
                    image: 'g1.png',
                },
                {   
                    image: 'g2.png',
                },
                {   
                    image: 'g3.png',
                },
                {   
                    image: 'g4.png',
                },
                {   
                    image: 'g5.png',
                },
                {   
                    image: 'g6.png',
                },
            ]
        }
     }
}
</script>