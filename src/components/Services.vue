<template>
  <div class="container-lg text-center">
    <div class="content d-flex justify-content-center flex-column">
        <h6>
            Mens grooming
        </h6>
        <h1>
            Services
        </h1>
    </div>
    <div class="row">
    <ServiceCard
    :services = 'services'
    />
    </div>
    <Button
    btnContent = 'Read about our services'
    />
  </div>
</template>

<script>
import Button from "./Commons/Button.vue";
import ServiceCard from "./Commons/ServiceCard.vue";
export default {
    components:{
        Button,
        ServiceCard,

    },
    data() {
        return {
            services:[
                {
                    service:'Trim & Cut',
                    description: 'Avada Barbers are experts in the lickety split trim and hair cut. Quick but careful and ridiculously good looking.',
                    img:'avadabarbers-trimcut-icon-before.png'
                },
                {
                    service:'Wash & Dry',
                    description: 'Take a seat in our fine leather chairs,lean back and let us lather you a fresh head in a luxurious fashion',
                    img:'avadabarbers-washndry-icon.png'
                },
                {
                    service:'Beard Tidy',
                    description: 'Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers',
                    img:'avadabarbers-beardtrim-icon.png'
                },

            ]
        }
    },

}
</script>

<style lang="scss">
@import '../assets/style/Colors.scss';
@import '../assets/style/MixIn.scss';

.content{
    margin: 0 auto;
    margin-top: 5rem;
    h1{
        color: $TextGrey;
        font-size: 5rem;
    }
}
    
</style>