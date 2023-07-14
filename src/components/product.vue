<script>
export default{
    data() {
        return {
        };
    },
    props: {
        productImage: String,
        productTitle: String
    }
};
</script>

<template>
    
        <div class="product">
            <div>
                <img
                :src="productImage"
                :alt="productTitle">
            </div>
            <h2>{{ productTitle }}</h2>
        </div>

</template>

<style scoped lang="scss">
.product{
    height: 200px;
    width: calc(100% / 6);
    h2{
            color: white;
        }
    div{
        img{
            width: 150px;
        }
        
    }
}

</style>