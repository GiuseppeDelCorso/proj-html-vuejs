<script>

export default {
    name: "AppMain1",
    data() {
        return {
            voteInt: (Math.ceil(this.cardInfo) / 2),
            cardInfo: [
                {
                    img: "186792_41e4_4-272x161",
                    typeCourses: "Development",
                    infoCourses: "The Complete iOS 10 & Swift 3 Developer Course",
                    price: "Free",
                    star: "20"
                },
                {
                    img: "246154_d8b0_3-272x161",
                    typeCourses: "Desing",
                    infoCourses: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
                    price: "100$",
                    star: 20
                },
                {
                    img: "1253188_58f7_2-272x161",
                    typeCourses: "Development",
                    infoCourses: "Web Design for Beginners: Real World Coding in HTML & CSS",
                    price: "65$",
                    star: 20
                },
                {
                    img: "1414956_d944_15-272x161",
                    typeCourses: "Desing",
                    infoCourses: "Digitally Painting Light and Color: Amateur to Master",
                    price: "70$",
                    star: 20
                },
                {
                    img: "1561458_7f3b-272x161",
                    typeCourses: "Art And Crafts",
                    infoCourses: "Become an Arabic Calligraphy Artist from Scratch",
                    price: "199$",
                    star: 20
                },
                {
                    img: "1776542_30b1-272x161",
                    typeCourses: "Google",
                    infoCourses: "Google Searching Ninja!",
                    price: "45$",
                    star: 20
                },

            ],

        }

    },

}




</script>

<template>
    <div class="container">
        <div class="row mt-4">
            <div class="col-6 bgRed">
                <h1 class="mt-6">Udemy Affilate Sales</h1>
                <p>Monetize your audience and attract new customers with Udemy!</p>
            </div>
            <div class="col-6 px-0">
                <img class="imgJuboStyle" src="../../public/img/slide-1.jpg" alt="">
            </div>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h4 class="py-4 fw-bold">Popular Development Courses</h4>
            </div>
        </div>
    </div>
    <div class="container mb-5">
        <div class="row">
            <div v-for="card in  cardInfo" class="col-2">
                <div class="card">
                    <img class="ImgCardStyle" :src="`../../public/img/${card.img}.jpg`">
                    <div class="styleCard">
                        <p class="styletypeCourses">{{ card.typeCourses }}</p>
                        <p class="styleinfoCourses">{{ card.infoCourses }}</p>
                        <hr>
                        <div class="d-flex px-3 ">
                            <i v-for="i in 5" :class="{ 'filled': i <= voteInt }" class="fas fa-star styleStar"></i>
                            <p class="styleprice">{{ card.price }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="container bgjubo2">
        <div class="row">
            <div class="col-12">
                <h1 class="styleTextJubo2">Limitless learning,<br> more possibilities</h1>
                <p class="styleParagrafJubo2">Online courses open the opportunity for learning to almost anyone, <br>
                    regardless of their scheduling
                    commitments
                </p>
                <button class="styleButton ">SIGN UP</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
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

.filled {
    color: #ff4450;
}

.styleStar {
    color: orange;
    font-size: 12px;
    padding: 4px;
}

.styleprice {
    margin-left: 35px;
    font-size: 15px;
    font-weight: bold;
}

.bgjubo2 {
    background-image: url(../../public/img/bg.png);
    height: 500px;
    background-position: center;
}

.styleTextJubo2 {
    font-weight: bold;
    padding-top: 150px;
    padding-left: 30px;
}

.styleParagrafJubo2 {
    padding-left: 30px
}

.styleButton {
    background-color: #ff4450;
    border: none;
    color: white;
    font-weight: bold;
    height: 40px;
    width: 100px;
    border-radius: 25px;
    font-size: 14px;
    margin-left: 30px
}
</style>
