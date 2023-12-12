<script>

export default {
    name: "CategoriesMain",
    props: {
        linkcategories: Object
    }
}




</script>

<template >
    <div class="container styleCategories">{{ this.linkcategories.type }}</div>
</template>

<style scoped>
.styleCategories {
    color: #333233;
    font-size: 12px;

}
</style>
