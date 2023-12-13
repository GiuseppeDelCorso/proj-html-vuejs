<script>

export default {
    name: "CategoriesMain",
    props: {
        linkcategories: Object
    }
}




</script>

<template >
    <div class="container styleCategories d-flex justify-content-center">
        <div class="row">
            <div class="col-12">
                <p>{{ this.linkcategories.type }}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.styleCategories {
    color: #333233;
    font-size: 12px;
    width: 100%;
    padding-top: 12px;
}

.styleCategories:hover {
    background-color: #457893;
    border-radius: 30px;
    color: white;
}
</style>
