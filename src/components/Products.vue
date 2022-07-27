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
        
    </div>
    <Button
    btnContent = 'Shop our product range'
    />
    </div>
  </div>
</template>

<script>
import Button from "./Commons/Button.vue";
export default {
    components:{
        Button
    },
    data() {
        return {
            products:[
                {
                    product:'Brush',
                    price:'15.00',
                    image:'brush_dark-600x600.png'
                },
                {
                    product:'Scissors',
                    price:'85.00',
                    image:'scissors-600x600.png'
                },
                {
                    product:'Hot Oil',
                    price:'15.00',
                    image:'hot_oil_dark-600x600.png'
                },
                {
                    product:'Straight Razor',
                    price:'30.00',
                    image:'straight_razor_dark-600x600.png'
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@import '../assets/style/Colors.scss';
@import '../assets/style/MixIn.scss';

#products{
    height: 100vh;
    margin: 2rem 0;
    padding-top: 8rem;
    background-image: url('../../public/Img/avadabarbers-reviewsbackground.jpg');
    background-size: cover;
    .content{
        h1{
            color: $TextGrey;
        }
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
/* #121314 */
    
</style>