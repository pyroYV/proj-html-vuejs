<template>
  <div id="about" class="d-flex text-center">
    <div class="content">
        <h6>Award Winning</h6>
        <h1>Pro Barbers</h1>
        <Button
        btnContent = 'Meet your new barber'
        />
    </div>
    <div class="triangle-bg"></div>
  </div>
</template>

<script>
import Button from "./Commons/Button.vue";
export default {
    components:{
        Button,
    }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/Colors.scss';

#about{
    height: 60vh;
    background-image: url('../../public/Img/avadabarbers-about-introbackground.jpg');
    background-size: cover;
    position: relative;
    .content{
        
        margin: 0 auto;
        margin-top: 10vh;
    }
    h1{
        font-family: 'Abril Fatface', sans-serif;
        font-size: 5rem;
        color: $TextWhite;
        margin-bottom: 3rem;
    }
    h6{
        color: $BrandColor;
        font-size: 1.5rem;
        font-weight: bold;
    }
    .triangle-bg{
    
    position: absolute;
    bottom: 0;
    border-style: solid;
    border-width: 0 50vw 100px 50vw;
    border-color: transparent transparent #ffffff transparent;
    display: inline-block;
    }
}
    
</style>