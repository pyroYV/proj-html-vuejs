<template>
  <div>
    <About />
    <Services />
    <Products />
    <Cta />
    <Reviews />
    <Blog />
  </div>
</template>

<script>
import About from "./About.vue";
import Services from "./Services.vue";
import Products from "./Products.vue";
import Cta from "./Cta.vue";
import Reviews from "./Reviews.vue";
import Blog from "./Blog.vue"

export default {
    components:{
        About,
        Services,
        Products,
        Cta,
        Reviews,
        Blog,

    }
    

}
</script>

<style lang="scss" scoped>

</style>