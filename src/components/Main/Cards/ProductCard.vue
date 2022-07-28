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
@import '../../../assets/style/Colors.scss';

.product{
    color:$BrandColor;
    text-align: center;
    *{
        margin-bottom: 1rem;
    }
    h3{
        font-family: 'Abril Fatface', sans-serif;
        font-size: 2rem;
        
    }
    p{
        font-size: 1.5rem        
    }
    img{
        width: 70%;
    }

}
    
</style>