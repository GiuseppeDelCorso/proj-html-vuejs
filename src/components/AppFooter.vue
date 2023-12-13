<script>

export default {
    name: "AppFooter",
}




</script>

<template>
    <div class="container bgdarck text-white">
        <div class="row">
            <div class="col-3">
                <p class="StyleTitle pt-4">ABOUT</p>
                <p class="styleText">Created by MasterStudy 2023. Sed nec felis pellentesque, lacinia dui sed, ultricies
                    sapien. Pellentesque
                    orci lectus, consectetur vel, rutrum eu ipsum. Mauris accumsan eros eget libero posuere vulputate.</p>
            </div>
            <div class="col-3">
                <p class="StyleTitle pt-4">CONTACT</p>
                <p class="styleText">USA, Callifornia 20, First Avenue, Callifornia</p>
                <p class="styleText">Tel.: +1 212 458 300 32 <br>
                    Fax: +1 212 375 24 14</p>
            </div>
            <div class="col-3">
                <p class="StyleTitle pt-4 ps-2">SOCIAL NETWORK</p>
                <div class="row">
                    <div class="col-12">
                        <i class="fa-brands fa-facebook style-logo"></i>
                        <i class="fa-brands fa-twitter style-logo"></i>
                        <i class="fa-brands fa-instagram style-logo"></i>
                        <i class="fa-brands fa-tiktok style-logo"></i>
                    </div>
                </div>
                <div class="row">
                    <div class="col-12">
                        <i class="fa-brands fa-discord style-logo"></i>
                        <i class="fa-brands fa-youtube style-logo"></i>
                        <i class="fa-brands fa-slack style-logo"></i>
                        <i class="fa-brands fa-apple style-logo"></i>
                    </div>
                </div>

            </div>
            <div class="col-3">
                <img class="styleImg" src="../../public/img/Top-udemy-courses-90-percent-off.jpg" alt="">
            </div>
        </div>
    </div>
</template>

<style scoped>
.styleText {
    font-size: 13px;
}

.StyleTitle {
    font-weight: bold;
    font-size: 16px;
}

.bgdarck {
    background-color: #263144;
}

.styleImg {
    width: 200px;
    height: 200px;
    object-fit: contain;
}

.style-logo {
    font-size: 25px;
    padding: 8px;
}
</style>
