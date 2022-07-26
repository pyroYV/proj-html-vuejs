<template>

  <div class="service">
    <img :src="item.img" alt="">
    <h3>{{item.service}}</h3>
    <p>
        {{item.description}}
    </p>
  </div>

</template>

<script>
export default {
    props:{
        item: Object,

    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/Colors.scss';
.service{
    *{
        margin-bottom: 2rem;
    }
    img{
        height: 10rem;
    }
    h3{
        font-family: 'Abril Fatface', sans-serif;
        font-size: 3rem;
        color:$BrandColor;
    }
    p{
        font-size: 1.3rem;
        line-height: 2rem;
        color: $TextGrey;
    }

}
</style>