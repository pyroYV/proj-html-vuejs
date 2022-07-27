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
    <div class="container-lg">
        
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/style/Colors.scss';
@import '../assets/style/Mixin.scss';
.content{
        margin: 0 auto;
    h1{
        font-family: 'Abril Fatface', sans-serif;
        font-size: 5rem;
        color: $TextGrey;
        margin-bottom: 3rem;
    }
    h6{
        color: $BrandColor;
        font-size: 1.5rem;
        font-weight: bold;
    }
}
</style>