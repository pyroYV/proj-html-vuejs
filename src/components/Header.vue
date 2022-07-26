<template>
<header>
    <Navbar />
    <Promos />
</header>
</template>

<script>
import Navbar from './Navbar.vue';
import Promos from './Promos.vue';


export default {
    name:'Header',
    components:{
        Navbar,
        Promos
    }
}
</script>

<style>

</style>