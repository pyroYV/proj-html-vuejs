<template>
  <div class="col-2">
    <ul>
        <a href="item.link" v-for="(item, index) in NavbarItems" :key="index">
          <li :class="item.class">

          </li>
        </a>
    </ul>
  </div>
</template>

<script>
export default {
    props:{
        NavbarItems: Array
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