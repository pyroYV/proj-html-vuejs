<template>
  <div class="container-fluid position-relative" id="products">
    <div class="triangle-bg">
    </div>
    <div class="content d-flex justify-content-center flex-column align-items-center">
        <h6>
            We have you covered
        </h6>
        <h1>
            Avada Grooming Products
        </h1>
    <div class="row">
    <ProductCard
        class="col-3"
        v-for="(item, index) in products" :key="index"
        :item = 'item'
    />
    </div>
    <Button
        btnContent = 'Shop our product range'
    />
    </div>
  </div>
</template>

<script>
import Button from "../Commons/Button.vue";
import ProductCard from "./Cards/ProductCard.vue";
export default {
    components:{
        Button,
        ProductCard,
    },
    data() {
        return {
            products:[
                {
                    product:'Brush',
                    price:'15.00',
                    img:'/img/brush_dark-600x600.png'
                },
                {
                    product:'Scissors',
                    price:'85.00',
                    img:'/img/scissors-600x600.png'
                },
                {
                    product:'Hot Oil',
                    price:'15.00',
                    img:'/img/hot_oil_dark-600x600.png'
                },
                {
                    product:'Straight Razor',
                    price:'30.00',
                    img:'/img/straight_razor_dark-600x600.png'
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@import '../../assets/style/Colors';
@import '../../assets/style/MixIn.scss';

#products{
    height: 110vh;
    margin: 2rem 0 0 0;
    padding-top: 8rem;
    background-image: url('../../../public/Img/avadabarbers-reviewsbackground.jpg');
    background-size: cover;
    .content{
        h1{
            color: $TextGrey;
        }
    }
    .row{
        margin-bottom: 4rem;
    }
    .triangle-bg{
    position: absolute;
    top: -99px;
    border-style: solid;
    border-width: 0 50vw 100px 50vw;
    border-color: transparent transparent #121314 transparent;
    display: inline-block;
    }
}

    
</style>