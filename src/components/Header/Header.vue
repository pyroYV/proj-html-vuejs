<template>
    <header class="position-relative">
        <div class="container-lg">
            <Navbar :NavbarItems="NavbarItems" />
            <div class="row p-2">
                <div class="col-7 d-flex flex-column justify-content-center hero-left">
                    <h1>
                        Barber Shop
                    </h1>
                    <span class="fs-3">The Pinnacle of Male Grooming</span>
                    <Button class="align-self-start" btnContent='Learn more' />
                </div>
                <div class="col-5">
                    <img src="/Img/avadabarbers_hero_focalmirror-800x1100.png" alt="Man getting a haircut">
                </div>

            </div>
        </div>
        <Promos saleprice='39' />
    </header>
</template>

<script>
import Navbar from './Navbar.vue';
import Promos from '../Commons/Promos.vue';
import Button from '../Commons/Button.vue';



export default {
    name:'Header',
    components:{
        Navbar,
        Promos,
        Button
    },
}
</script>

<style lang="scss"scoped>@import '../../assets/style/Colors';

header {
    height: 90vh;
    color: white;
    background-image: url('../../../public/Img/avadabarbers-homepage-hero-bg.jpg');
    background-position: top;
    background-size: cover;
    background-repeat: no-repeat;

    h1 {
        font-family: 'Abril Fatface', sans-serif;
        font-size: 6.5rem;
        padding: 2rem 0;
        position: relative;
        color: $TextWhite !important;

        &:before {
            content: '';
            width: 275px;
            height: 5px;
            background-color: $BrandColor;
            position: absolute;
            bottom: 0;

        }
    }

    .hero-left>* {
        margin-bottom: 2.5rem;
        color: $TextGrey;
    }

    .col-5 {
        img {
            width: 100%;
        }
    }

}

</style>