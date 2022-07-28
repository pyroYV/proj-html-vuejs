<template>
  <div id="arrow-up" class="position-absolute rounded" @click="scrollToTop()">
    <i class="bi bi-arrow-bar-up"></i>
  </div>
</template>

<script>
export default {
    methods: {
        scrollToTop() {
            window.scrollTo(0, 0);
        },
    },
}
</script>

<style>
#arrow-up{
    bottom: 0;
    right: 3%;
    padding: .4rem 1rem;
    font-size: 1.5rem;
    background-color: #303030;
    color: white;
    cursor: pointer;
}
</style>