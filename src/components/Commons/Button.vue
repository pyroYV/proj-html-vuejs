<template>

  <a href="#" class="bottone">
    {{btnContent}}
  </a>

</template>

<script>
export default {
    props:{
        btnContent: String
    }
}
</script>

<style lang ="scss" scoped>
@import '../../assets/style/Colors.scss';


.bottone{
    text-align: center;
    padding: 0.8rem 2.5rem;
    border: 3px solid;
    border-color: $BrandColor;
    color: $BrandColor !important;
    font-size: 1.5rem;
    text-transform: uppercase;
    &:hover{
      color:$BrandHover !important;
      border-color: $BrandHover;
    }
}
</style>