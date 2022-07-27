<template>
  <div id="cta">
    <div class="container-lg">
        <div class="row">
            <div class="col-5 d-flex justfy-content-center align-items-center">
                <div class="bg-image">
                    <img src="../../public/Img/avadabarbers-second-blog-700x441.jpg" alt="">
                </div>
                <div class="image">
                <img src="../../public/Img/shaving_butter-600x600.png" alt="Shaving Butter" >
                </div>
            </div>
            <div class="col-7">
                allora
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/style/Colors.scss';

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
                        width: 600px;
                        filter: grayscale(100%);
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
    }


</style>