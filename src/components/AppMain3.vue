<script>

export default {
    name: "AppMain3",
}




</script>

<template>
    <div class="container bgred pb-2 mb-5">
        <div class="row">
            <div class="col-6 py-2">
                <p class="styleTitle pt-3">Subscribe our newsletter</p>
                <p class="styleText">There are many variations of passages of Lorem Ipsum available, but the majority have
                    suffered
                    <br>alteration in some form, by injected humour, or randomised words
                </p>
            </div>
            <div class="col-6 py-2">
                <p class="text-white pt-3">YOUR E-MAIL ADDRESS</p>
                <div class="input-group mb-3">
                    <input type="text" class="form-control" placeholder="Recipient's username"
                        aria-label="Recipient's username" aria-describedby="basic-addon2">
                    <span class="input-group-text prova" id="basic-addon2">SUBSCRIBE</span>
                </div>
            </div>
        </div>
    </div>
    <div class="container mb-4 pt-5">
        <div class="row">
            <div class="col-12">
                <h1 class="text-center fw-bold">Popular courses</h1>
                <p class="text-center styleText2">Discover our most popular courses for self learning</p>
            </div>
        </div>
    </div>
</template>

<style scoped> .bgred {
     background-color: #ff4450;
 }

 .styleTitle {
     color: white;
     font-weight: bold;
 }

 .styleText {
     color: white;
     font-size: 14px;
 }

 .styleText2 {
     color: #b3b2b3;
 }

 .prova {
     background-color: #447993;
     border: none;
     color: white;
 }
</style>