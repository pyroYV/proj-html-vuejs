<template>
    <div class="blog-post">
        <img :src="item.img" :alt="item.imgAlt">
        <h3>{{item.title}}</h3>
        <p>
            {{item.post}}
        </p>
    </div>
</template>

<script>
export default {
    props:{
        item: Object,
    },
}
</script>

<style lang="scss"scoped>@import '../../../assets/style/Colors.scss';

.blog-post {

    * {
        margin-bottom: 1.5rem;
        padding: 0 1rem;

    }

    img {
        height: 15rem;
    }

    h3 {
        font-family: 'Abril Fatface', sans-serif;
        font-size: 2.5rem;
        color: $BrandColor;
    }

    p {
        font-size: 1.2rem;
        line-height: 2rem;
        color: $TextGrey;
    }

}

</style>