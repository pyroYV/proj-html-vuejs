<template>
  <div id="cta">
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

#cta{
    height: 50vh;
    position: relative;

    .container-lg{
        position: absolute;
        color: $TextGrey;
        background-color: $DarkGrey;
        border-top: 10px solid;
        border-color: $BrandColor;
        height: 45vh;
        top: -5rem;
        left: 0; 
        right: 0; 
        margin-left: auto; 
        margin-right: auto; 
    }
}

</style>