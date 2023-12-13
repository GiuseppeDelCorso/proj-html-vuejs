<script>

export default {
    name: "AppMain4",
}




</script>

<template>
    <div class="container">
        <div class="row d-flex ">
            <div class="col-6">
                <div class="row styleBorder d-flex">
                    <div class="col-4">
                        <img class="styleImg" src="../../public/img/image_box_1-221x231.png" alt="">
                    </div>
                    <div class="col-8 mt-6 ">
                        <h2>Become an Instructor</h2>
                        <p>Teach what you love. Masterstudy gives you the tools to create a course.</p>
                        <button class="styleButton">START TEACHING</button>
                    </div>

                </div>
            </div>
            <div class="col-6">
                <div class="row styleBorder d-flex">
                    <div class="col-4">
                        <img class="styleImg" src="../../public/img/image_box_2-234x231.png" alt="">
                    </div>
                    <div class="col-8 mt-6 ">
                        <h2>Access For Business</h2>
                        <p>Get unlimited access to 2,500 of top courses <br> for your team.</p>
                        <button class="styleButton">DOING BUISNESS</button>
                    </div>

                </div>
            </div>
        </div>
    </div>
    <div class="container bgjubo2 mt-5">
        <div class="row ">
            <div class="col-12 styleBox">
                <h1 class="styleTextJubo2">Paints of the Future</h1>
                <p class="styleParagrafJubo2">The response to your MasterStudy has been really overwhelming! Those who
                    participated in the workshop are spreading the word here on campus and the “buzz” is on. The VP of
                    Instruction wants you to come back! Her goal is to have more faculty trained. She also wants to attend a
                    workshop herself. Our President told me Masterstudy needs to be the cornerstone of our success program.”
                </p>
                <p class="styleName">Linda Green <br>
                    Product Manager, Apple Inc</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
h2 {
    font-weight: bold;
}

p {
    font-size: 15px;
    color: #b3b2b3;
}

.styleImg {
    width: 150px;
    height: 150px;
    margin-top: 80px;
    object-fit: contain;
}

.styleButton {
    background-color: #ff4450;
    border: none;
    color: white;
    font-weight: bold;
    height: 50px;
    width: 150px;
    border-radius: 25px;
    font-size: 12px;
}

.styleButton:hover {
    background-color: #457893;
    border-radius: 30px;
    color: white;
}

.styleBorder {
    border: 1px solid rgb(223, 217, 217);
    height: 300px;
    width: 660px;
}

.mt-6 {
    margin-top: 80px;
}

.bgjubo2 {
    background-image: url(../../public/img/testimonial-1-1917x640-1-1914x639.jpg);
    height: 500px;
    background-position: center;
}

.styleTextJubo2 {
    padding: 30px;
}

.styleParagrafJubo2 {
    padding: 20px;
}

.styleBox {
    margin: 40px 0 0 80px;
    width: 450px;
    background-color: white;
}

.styleName {
    padding: 0 0 30px 20px;
}
</style>