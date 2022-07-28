<template>
  <footer>
    <div class="container-lg">
        <div class="row p-5 text-center">
            <div class="col-4 d-flex flex-column p-4">
                <img src="/img/avadabarbers_footer_shop_image-600x468.png" alt="Beard products kit">
                <Button 
                    class="align-self-center"
                    fs = 'fs-5'
                    btnContent="Shop our range now"
                />
            </div>
            <div class="col-4 d-flex flex-column justify-content-center align-items-center middle">
                <img src="/img/avadabarbers-logo-x1.png" alt="Avada barbers logo">
                <div class="info mt-5">
                    <p>Avada Barbers</p>
                    <p>123 New York Street</p>
                    <p>New York City</p>
                    <p>Info@yourwebsite.com</p>
                    <p>+1 (555) 555-1212</p>
                </div>
                <h5>
                    Follow us
                </h5>
                <div class="socials">
                    <ul>
                        <a href="item.link" v-for="(item, index) in socials" :key="index">
                            <li :class="item.class">
                            </li>
                        </a>
                    </ul>
                </div>
            </div>
            <div class="col-4 d-flex flex-column p-4">
                <img src="/img/avadabarbers_footer_appointment_image-600x468.png" alt="Man getting haircut">
                <Button 
                    class="align-self-center"
                    btnContent="Book your appointment"
                    fs = 'fs-5'
                />
            </div>
        </div>
    </div>
        <div class="text-center d-flex justify-content-center align-items-center position-relative" id="copyright">
            <p>
              &copy; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress
            </p>
    <ToTop
    
    />
        </div>
  </footer>
</template>

<script>
import Button from "../Commons/Button.vue";
import ToTop from '../Commons/ToTop.vue';
export default {
    components:{
        Button,
        ToTop,
    },
    data() {
        return {
            socials:[
                {
                    name:'Facebook',
                    class:'bi bi-facebook',
                    link:'#'
                },
                {
                    name:'Twitter',
                    class:'bi bi-twitter',
                    link:'#'
                },
                {
                    name:'Youtube',
                    class:'bi bi-youtube',
                    link:'#'
                },
                {
                    name:'Instagram',
                    class:'bi bi-instagram',
                    link:'#'
                },
            ]
        }
    },

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/Colors.scss';

footer{
    height: 60vh;
    background-color: #121314;
    color: $TextFooter;
    #copyright{
        height: 10vh;
        background-color: #161718;
    }
    .middle{
        img{
            width: 50%;
        }
        
        line-height: 0.5rem;
        h5{
            color:$BrandColor;
            text-transform: uppercase;
            margin: 2rem 0;
        }
        ul{
            padding: 0;
            li{
                font-size: 1rem;
            &:hover{
                color: $BrandColor;
            }
            }
        }
    }
}
</style>