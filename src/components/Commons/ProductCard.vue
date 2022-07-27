<template>
  <div class="product">
    <img :src="item.img" alt="">
    <h3>{{item.product}}</h3>
    <p>
        ${{item.price}}
    </p>
  </div>
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

.product{
    color:$BrandColor;
    text-align: center;
    *{
        margin-bottom: 2rem;
    }
    h3{
        font-family: 'Abril Fatface', sans-serif;
        font-size: 3rem;
        
    }
    p{
        font-size: 1.8rem;
        line-height: 2rem;
        
    }

}
    
</style>