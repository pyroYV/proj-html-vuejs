<template>
<div id="promos">
    <div class="promotion p-2 px-3 text-center rounded mb-2"> 
    <div><i class="bi bi-terminal-fill"></i></div>
    <div>
        Demos
    </div>
  </div>
  <div class="promotion p-2 px-3 text-center rounded"> 
        <div class="sale-price">{{saleprice}}</div>
        <div>
            On Sale
        </div>
  </div>
</div>
</template>

<script>
export default {
    props:{
        saleprice: String
    }
}
</script>

<style lang="scss">
@import '../assets/style/Colors.scss';

#promos{
    position: fixed;
    right: 1%;
    top: 12%;
    color: #33475b;
    z-index: 3;
    .promotion{
        background-color: white;
        font-weight: bolder;
        .sale-price{
            color: $HighlightGreen;
            font-size: 2.2rem;
            position: relative;
            &:before{
                content: '$';
                position:absolute;
                left: -5px;
                top: 0;
                font-size: 1.2rem;

            }   
        }
        i{
            font-size: 1.6rem;
        }
    }
    
}
</style>