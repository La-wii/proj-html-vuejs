<template>
    <!-- start section -->
    <div class="youtube-section py-5">
        <!-- start container -->
        <div class="container-lg">
            <!-- start row -->
            <div class="row">
                <!-- start col -->
                <div class="col-6 position-relative">

                    <div class="top-green-decoration">
                        <img src="/img/pallini-verdi-rotonda.png" alt="pallini verdi png">
                    </div>
                    
                    <div class="img-poster">
                        <img src="/img/video-poster.jpg" alt="video">
                    </div>

                    <div class="youtube-icon">
                        <img src="/img/icon-youtube-play.png" alt="play video">
                    </div>

                    <div class="green-decoration">
                        <img src="/img/pallini-verdi-150.png" alt="">
                    </div>
                    
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-6 p-5">
                    
                    <div class="content p-5">
                        <p class="text-uppercase">
                        get started
                            <strong>
                                effortlessly
                            </strong>
                        </p>

                        <h2 class="text-capitalize display-6 py-2">
                            enjoy our
                            <span class="text-capitalize">companionship</span> 
                        </h2>

                        <p class="gr">
                            Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.
                        </p>

                        <a href="#">
                            Download free guidebook
                            <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                    
                </div>
                <!-- end col -->


            </div>
            <!-- end row -->
        </div>
        <!-- end container -->
    </div>
    <!-- end section -->
</template>

<script>
export default {
    name: "Youtube",
}
</script>

<style scoped lang="scss">
    .youtube-section{
        // height: 500px;
        .container-lg{
            .row{
                .col-6{
                    .top-green-decoration{
                        position: absolute;
                        z-index: -10;
                        left: -10%;
                        top: -5%;
                    }
                    // .img-poster{
                        
                    // }
                    .youtube-icon{
                        position: absolute;
                        left: 50%;
                        top: 50%;
                        transform: translate(-50%,-50%);
                    }
                    .green-decoration{
                        position: absolute;
                        right: -10%;
                        bottom: -5%;
                        z-index: -10;
                    }
                }

                .col-6{
                    p{
                        font-size: 20px;
                    }
                    h2{
                        span{
                            color: #20AD96;
                        }
                    }
                    .gr{
                        font-size: 20px;
                        color: #aeadae;
                    }
                    a{
                        color: #20AD96;
                        font-size: 18px;
                    }
                }
            }
        }
    }
</style>