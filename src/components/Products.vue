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