<template>
    <div class="product-card">
        <img :src="immage" :alt="title">
        <h3>{{ title }}</h3>
    </div>

</template>

<script>

export default{
    props: {
        immage: String,
        title: String
    }

}

</script>

<style lang="scss" scoped>
.product-card {
    & img{
        width: 80%;
        height: 178px;
    }
    & h3{
        font-size: 12px;
        color: white;
        padding: 16px 0px;
    }
}

</style>