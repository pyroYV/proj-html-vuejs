<template>
  <div class="row justify-content-between pt-4">
    <div class="col-1 ps-4">
      <img id="header-logo" src="/Img/avadabarbers-logo-x1.png" alt="Avada Barbers logo">
    </div>
    <div class="col-2">
      <ul>
        <a href="item.link" v-for="(item, index) in NavbarItems" :key="index">
          <li :class="item.class">
          </li>
        </a>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    data() {
      return {
          NavbarItems:[
                {
                    item:1,
                    link:"#",
                    class:'bi bi-cart-fill'

                },
                {
                    item:2,
                    link:'#',
                    class:'bi bi-list bi-2x'
                }
            ],
      }
    },

}
</script>

<style lang="scss">@import '../../assets/style/Colors.scss';

ul{
  li{
    padding: 0.5rem;
    font-size: 2rem;
    &:hover{
                color: $BrandColor;
            }
  }
}
</style>