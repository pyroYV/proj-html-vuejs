<template>
<header>
    <div class="container-lg">
    <div class="row justify-content-between pt-4">
        <div class="col-1">
        <img id="header-logo" src="../../public/Img/avadabarbers-logo-x1.png" alt="">
        </div>
        <Navbar
        :NavbarItems = NavbarItems
         />
    </div>
    </div>
    <Promos />
</header>
</template>

<script>
import Navbar from './Navbar.vue';
import Promos from './Promos.vue';


export default {
    name:'Header',
    components:{
        Navbar,
        Promos
    },
    data() {
        return {
            NavbarItems:[
                //navbar due item o tre ? il logo è compreso?
            /*     {
                    item:0,
                    link:'#',
                    image:'../../public/Img/avadabarbers-logo-x1.png'
                }, */
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

        }
    },
}
</script>

<style lang="scss">
    header{
        height: 100vh;
        color: white;
        background-image: url('../../public/Img/avadabarbers-homepage-hero-bg.jpg');
        background-position: top;
        background-size: cover;
        background-repeat: no-repeat;
    }
</style>