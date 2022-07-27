<template>
  <div>
    <About />
    <Services />
    <Products />
    <Cta />
  </div>
</template>

<script>
import About from "./About.vue";
import Services from "./Services.vue";
import Products from "./Products.vue";
import Cta from "./Cta.vue";

export default {
    components:{
        About,
        Services,
        Products,
        Cta

    }
    

}
</script>

<style lang="scss" scoped>

</style>