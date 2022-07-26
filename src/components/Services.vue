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
                    description: ''
                }
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