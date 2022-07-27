<template>
  <div>
    <About />
    <Services />
    <Products />
  </div>
</template>

<script>
import About from "./About.vue";
import Services from "./Services.vue";
import Products from "./Products.vue";

export default {
    components:{
        About,
        Services,
        Products

    }
    

}
</script>

<style lang="scss" scoped>

</style>