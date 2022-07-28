<template>
    <div class="d-flex text-center flex-column mt-5" id="reviews">
        <div class="content">
            <h6>
                What people say
            </h6>
            <h1>
                Reviews
            </h1>
        </div>
        <div class="container-lg mt-5">
            <div class="row justify-content-center">
                <ReviewCard class="col-3 me-5" v-for="(item, index) in reviews" :key="index" :item='item' />
            </div>
        </div>
        <div class="triangle-bg">
        </div>
    </div>
</template>

<script>
import ReviewCard from "./Cards/ReviewCard.vue";

export default {
    components:{
        ReviewCard,
    },
    data() {
        return {
            reviews:[
                {
                    name:'John Doe',
                    review: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, deleniti vel animi culpa facere autem incidunt possimus, a quo reprehenderit sequi quaerat corporis, molestiae eaque ullam eos. Officia, ex quam!',
                    img:'/img/avadabarbers-trimcut-gallery6-400x400.jpg'
                },
                {
                    name:'Pete Jones',
                    review: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, deleniti vel animi culpa facere autem incidunt possimus, a quo reprehenderit sequi quaerat corporis, molestiae eaque ullam eos. Officia, ex quam!',
                    img:'/img/avadabarbers-trimcut-gallery7-400x402.jpg'
                },
                {
                    name:'Mark Wilson',
                    review: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero, deleniti vel animi culpa facere autem incidunt possimus, a quo reprehenderit sequi quaerat corporis, molestiae eaque ullam eos. Officia, ex quam!',
                    img:'/img/avadabarbers-trimcut-gallery3-400x402.jpg'
                },
            ]
        }
    },
}
</script>

<style lang="scss"scoped>@import '../../assets/style/Colors.scss';
@import '../../assets/style/Mixin.scss';

#reviews {
    height: 100vh;
    padding-top: 10vh;
    position: relative;

    .content {
        margin: 0 auto;

        h1 {
            font-family: 'Abril Fatface', sans-serif;
            font-size: 5rem;
            color: $TextGrey;
            margin-bottom: 3rem;
        }

        h6 {
            color: $BrandColor;
            font-size: 1.5rem;
            font-weight: bold;
        }
    }

    .triangle-bg {
        position: absolute;
        bottom: -100px;
        border-style: solid;
        border-width: 100px 50vw 0 50vw;
        border-color: white transparent transparent transparent;
        display: inline-block;
    }
}

</style>