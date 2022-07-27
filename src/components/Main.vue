<template>
  <div>
    <About />
    <Services />
    <Products />
    <Cta />
    <Reviews />
  </div>
</template>

<script>
import About from "./About.vue";
import Services from "./Services.vue";
import Products from "./Products.vue";
import Cta from "./Cta.vue";
import Reviews from "./Reviews.vue";

export default {
    components:{
        About,
        Services,
        Products,
        Cta,
        Reviews

    }
    

}
</script>

<style lang="scss" scoped>

</style>