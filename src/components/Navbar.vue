<template>
<div class="row justify-content-between pt-4">
    <div class="col-1 ps-4">
      <img id="header-logo" src="../../public/Img/avadabarbers-logo-x1.png" alt="">
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
    props:{
        NavbarItems: Array,
        prova: String
    }

}
</script>

<style lang="scss">

ul{
  li{
    padding: 0.5rem;
    font-size: 1.5rem;
  }
}
</style>