<template>
  <div id="cta">
    <div class="container-lg">
        <div class="row">
            <div class="col-5 d-flex justfy-content-center align-items-center">
                <div class="bg-image">
                    <img src="/Img/avadabarbers-second-blog-700x441.jpg" alt="">
                </div>
                <div class="image">
                <img src="/Img/shaving_butter-600x600.png" alt="Shaving Butter" >
                </div>
            </div>
            <div class="col-7">
            <h6>
                this months featured product
            </h6>
            <h1>
                Shaving Butter
            </h1>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore laudantium libero dolore velit. Quis dolore aperiam ea a magnam! Quam eos voluptate soluta praesentium quod odio doloribus consectetur corporis enim!
            </p>
            <div class="pt-4">
                <Button
                btnContent = 'buy now'
                />
            </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import Button from './Commons/Button.vue'
export default {
        components:{
            Button
        }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/Colors.scss';
@import '../assets/style/MixIn.scss';


#cta{
    height: 50vh;
    position: relative;

    .container-lg{
        position: absolute;
        color: $TextGrey;
        background-color: $DarkGrey;
        border-top: 10px solid;
        border-color: $BrandColor;
        height: 35rem;
        top: -5rem;
        left: 0; 
        right: 0; 
        margin-left: auto; 
        margin-right: auto;
        .col-5{
            padding: 0; 
            position: relative;   
            .bg-image{
                    img{
                        height: 552px;
                        width: 550px;
                        filter: grayscale(100%) opacity(50%);
                    }     
                }
            }
            .image{
            position: absolute;
            left: 0; 
            right: 0; 
            margin-left: auto; 
            margin-right: auto;
            img{
                width: 100%;
                height: 100%;
            }
            }
        }
        .col-7{
            padding:4rem 6rem;
            line-height: 2.5rem;
        }
    }


</style>