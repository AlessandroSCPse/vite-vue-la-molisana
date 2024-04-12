<script>
export default {
    name: 'ProductCard',
    props: {
        cardInfo: Object
    }
    // props: ['cardInfo']
}
</script>

<template>
    <div class="product-card">
        <div>
            <img :src="cardInfo.src">
        </div>

        <h3>{{ cardInfo.titolo }}</h3>
    </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

.product-card {
    background-color: white;
    padding: 10px;
    width: calc((100% / 4) - 6px);
    margin: 3px 0;

    h3 {
        text-align: center;
        color: $brand-primary;
    }
}
</style>