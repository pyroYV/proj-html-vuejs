<template>
<div class="review">
    <p>
        {{item.review}}
    </p>
    <img :src="item.img" alt="">
    <h5 class="name"> {{item.name}} </h5>
  </div>

</template>
</template>

<script>
export default {
    props:{
        item: Object
    }

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/Colors.scss';

.review{
    padding: 0 1rem;
    *{
        margin-bottom: 2rem;
    }
    img{
        height: 10rem;
        border-radius: 50%;
    }
    h5{
        font-family: 'Lato', sans-serif;
        font-weight: 400;
        font-style: italic;
        color:$BrandColor;
    }
    p{
        font-size: 1rem;
        line-height: 2rem;
        color: $TextGrey;
    }

}
</style>