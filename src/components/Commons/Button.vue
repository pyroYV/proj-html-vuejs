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
.bottone{
    text-align: center;
    padding: 0.8rem 2.5rem;
    border: 2px solid;
    border-color: #ae8652;
    color: #ae8652 !important;
    font-size: 1.5rem;
    text-transform: uppercase;
}
</style>