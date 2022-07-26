<template>
<header class="position-relative">
    <div class="container-lg">
            <Navbar
            :NavbarItems = "NavbarItems"
            />
        <div class="row p-2">
            <div class="col-6 d-flex flex-column justify-content-center hero-left">
                <h1>
                    Barber Shop
                </h1>
                <span class="fs-5">The Pinnacle of Male Grooming</span> 
                <Button
                class="align-self-start"
                btnContent = 'Learn more'
                 />
            </div>
            <div class="col-6">
                <img src="../../public\Img\avadabarbers_hero_focalmirror-600x825.png" alt="">
            </div>

        </div>
    </div>
    <Promos 
    saleprice = '39'
    />
</header>
</template>

<script>
import Navbar from './Navbar.vue';
import Promos from './Promos.vue';
import Hero from './Hero.vue';
import Button from './Commons/Button.vue';



export default {
    name:'Header',
    components:{
        Navbar,
        Promos,
        Hero,
        Button
    },
    data() {
        return {
            NavbarItems:[
                {
                    item:1,
                    link:"#",
                    class:'bi bi-cart-fill'

                },
                {
                    item:2,
                    link:'#',
                    class:'bi bi-list bi-2x'
                }
            ],
            Logopath:""

        }
    },
}
</script>

<style lang="scss" scoped>
@import '../assets/style/Colors.scss';

    header{
        height: 100vh;
        color: white;
        background-image: url('../../public/Img/avadabarbers-homepage-hero-bg.jpg');
        background-position: top;
        background-size: cover;
        background-repeat: no-repeat;
        h1{
            font-family: 'Abril Fatface', sans-serif;
            font-size: 6rem;
            padding: 2rem 0;
            position: relative;
            color: $TextWhite;
            
            &:before{
                content: '';
                width: 275px;
                height: 5px;
                background-color: $BrandColor;
                position: absolute;
                bottom: 0;

            }
        }
        .hero-left>*{
            margin-bottom: 1rem;
            color: $TextGrey;
        }

    }
</style>