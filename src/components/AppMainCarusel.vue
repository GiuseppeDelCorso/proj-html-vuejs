<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/free-mode';
import 'swiper/css/pagination';


// import required modules
import { FreeMode, Pagination } from 'swiper/modules';

export default {
    props: {
        linksCards: Object
    },
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {

        return {
            modules: [FreeMode, Pagination],
            cardInfo: [
                {
                    img: "186792_41e4_4-272x161",
                    typeCourses: "Development",
                    infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
                    price: "Free",
                    star: 4
                },
                {
                    img: "246154_d8b0_3-272x161",
                    typeCourses: "Desing",
                    infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
                    price: "100$",
                    star: 5
                },
                {
                    img: "1253188_58f7_2-272x161",
                    typeCourses: "Development",
                    infoCourses: "Web Design for Beginners: Real World Coding in HTML & CSS",
                    price: "65$",
                    star: 3
                },
                {
                    img: "1414956_d944_15-272x161",
                    typeCourses: "Desing",
                    infoCourses: "Digitally Painting Light and Color: Amateur to Master",
                    price: "70$",
                    star: 1
                },
                {
                    img: "1561458_7f3b-272x161",
                    typeCourses: "Art And Crafts",
                    infoCourses: "Become an Arabic Calligraphy Artist from Scratch",
                    price: "199$",
                    star: 4
                },
                {
                    img: "1776542_30b1-272x161",
                    typeCourses: "Google",
                    infoCourses: "Google Searching Ninja! GO GO GO!",
                    price: "45$",
                    star: 4
                },
                {
                    img: "838056_611a_3-272x161",
                    typeCourses: "Development",
                    infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
                    price: "Free",
                    star: 5
                },
                {
                    img: "895786_7b4b_2-272x161",
                    typeCourses: "Desing",
                    infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
                    price: "100$",
                    star: 3
                },
                {
                    img: "919872_ed54_6-272x161",
                    typeCourses: "Development",
                    infoCourses: "Web Design for Beginners: Real World Coding in HTML & CSS",
                    price: "65$",
                    star: 2
                },
                {
                    img: "949316_2a64_11-272x161",
                    typeCourses: "Desing",
                    infoCourses: "Digitally Painting Light and Color: Amateur to Master",
                    price: "70$",
                    star: 4
                },
                {
                    img: "951684_9c1a_2-272x161",
                    typeCourses: "Art And Crafts",
                    infoCourses: "Become an Arabic Calligraphy Artist from Scratch",
                    price: "199$",
                    star: 2
                },
                {
                    img: "1208228_d61c_4-272x161",
                    typeCourses: "Google",
                    infoCourses: "Google Searching Ninja! GO GO GO!",
                    price: "45$",
                    star: 3
                },
                {
                    img: "838056_611a_3-272x161",
                    typeCourses: "Development",
                    infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
                    price: "Free",
                    star: 5
                },
                {
                    img: "895786_7b4b_2-272x161",
                    typeCourses: "Desing",
                    infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
                    price: "100$",
                    star: 3
                },

            ],
        };
    },
};




</script>
<template>
    <div class="container mb-4 bgContainer">
        <div class="row">
            <div class="col-12">
                <swiper :slidesPerView="6" :spaceBetween="30" :freeMode="true" :pagination="{
                    clickable: true,
                }" :modules="modules" class="mySwiper">
                    <swiper-slide v-for="img in cardInfo">
                        <div class="row my-3">
                            <div class="col-2">
                                <div class="card">
                                    <img class="ImgCardStyle" :src="`../../public/img/${img.img}.jpg`">
                                    <div class="styleCard">
                                        <p class="styletypeCourses">{{ img.typeCourses }}</p>
                                        <p class="styleinfoCourses">{{ img.infoCourses }}</p>
                                        <hr>
                                        <div class="d-flex px-3 ">
                                            <i v-for="i in 5" :class="{ 'filled': i <= img.star }"
                                                class="fas fa-star styleStar"></i>
                                            <p class="styleprice">{{ img.price }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                </swiper>
            </div>
        </div>
    </div>
</template>

<style scoped>
.bgContainer {
    background-color: #f1f4fb;
}

.mt-6 {
    margin-top: 110px;
}

.bgRed {
    background-color: #ff4450;
    color: white;
}

.imgJuboStyle {
    width: 100%;
    height: 350px;
    object-fit: cover;

}

.card {
    width: 210px;
}

.styleCard {
    height: 200px;
    width: 200px;
}

.ImgCardStyle {
    width: 210px;
    height: 120px;
    object-fit: cover
}

.styletypeCourses {
    color: #b3b2b3;
    font-size: 12px;
    padding: 10px 0 5px 10px;
}

.styleinfoCourses {
    font-size: 12px;
    padding: 0px 10px 0px 10px;
}

hr {
    width: 85%;
    margin-left: 16px;
}


.styleStar {
    color: lightgrey;
    font-size: 12px;
    padding: 4px;
}

.filled {
    color: orange;
}

.styleprice {
    margin-left: 35px;
    font-size: 15px;
    font-weight: bold;
}
</style>