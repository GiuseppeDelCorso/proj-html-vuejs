<script>

export default {
    name: "AppMain2",
    props: {
        linksCards: Object
    }
}




</script>

<template>
    <div class="row my-3">
        <div class="col-2">
            <div class="card">
                <img class="ImgCardStyle" :src="`../../public/img/${linksCards.img}.jpg`">
                <div class="styleCard">
                    <p class="styletypeCourses">{{ linksCards.typeCourses }}</p>
                    <p class="styleinfoCourses">{{ linksCards.infoCourses }}</p>
                    <hr>
                    <div class="d-flex px-3 ">
                        <i v-for="i in 5" :class="{ 'filled': i <= linksCards.star }" class="fas fa-star styleStar"></i>
                        <p class="styleprice">{{ linksCards.price }}</p>
                    </div>
                </div>
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
