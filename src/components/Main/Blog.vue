<template>
  <div class="d-flex text-center flex-column" id="blog">
    <div class="content">
      <h6>
        Tales from the barber shop
      </h6>
      <h1>
        Recent Blog Posts
      </h1>
    </div>
    <div class="container-lg">
      <div class="row">
        <BlogPost class="col-4" v-for="(item, index) in blogposts" :key="index" :item='item' />
      </div>
    </div>
    <Button class="align-self-center mt-5" btnContent="Read more from our blog" />
  </div>
</template>

<script>
import Button from "../Commons/Button.vue";
import BlogPost from "./Cards/BlogPostCard.vue";

export default {
  components:{
    Button,
    BlogPost,
  },
    data() {
      return {
        blogposts:[
            {
            title:'Avada Barbers Now Open',
            post:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Distinctio culpa optio molestiae ad maiores?',
            img:'/img/avadabarbers-second-blog-700x441.jpg',
            imgAlt:'Barber shop poles'

            },
            {
            title:'Choosing The Right Barber',
            post:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Distinctio culpa optio molestiae ad maiores?',
            img:'/img/avadabarbers-choosing-blog-320x202.jpg',
            imgAlt:'Barber shop chairs'
            

            },
            {
            title:'Quick Service Guide',
            post:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Distinctio culpa optio molestiae ad maiores?',
            img:'/img/avadabarbers-ourservice-blog-320x202.jpg' ,
            imgAlt:"Barber trimming client's beard"       

            },
        ]
    }
  },
  
}
</script>

<style lang="scss"scoped>@import '../../assets/style/Colors.scss';
@import '../../assets/style/Mixin.scss';

#blog {
  background-color: $TextWhite;
  height: 120vh;
  padding-top: 20vh;

  h1 {
    color: $TextGrey;
  }

  h6 {
    font-size: 1rem;
  }
}

</style>