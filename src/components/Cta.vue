<template>
    <div class="cta-section py-5">
        <!-- start container -->
        <div class="container-lg">
            <div class="row">
                <!-- start col -->
                <div class="col-2">
                    
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-8 text-center position-relative">
                    <h4 class="py-3">Start today for getting <span>Online Certification</span></h4>
                    <h2 class="pb-5 display-6">You can be your own guiding star with our help!</h2>
                    <button class="btn-green">
                        Get started now
                    </button>
                    <img src="/img/righe.png" alt="righe" class="righe">
                    <img src="/img/cerchio.png" alt="cerchio" class="cerchio">
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-2">

                </div>
                <!-- end col -->
            </div>
        </div>
        <!-- end container -->
    </div>
</template>

<script>
export default {
    name: "Cta",
}
</script>

<style scoped lang="scss">
    .cta-section{
        background-color: #f6f3f5;
            .container-lg{
                .row{
                    // .col-2{

                    // }
                    .col-8{
                        h4{
                            span{
                                color: #20AD96;
                            }
                        }
                        .cerchio{
                            width: 100px;
                            position: absolute;
                            right: -15%;
                            bottom: 0;
                        }
                        .righe{
                            width: 180px;
                            position: absolute;
                            left: -25%;
                            bottom: 20%;
                        }
                        // h2{
                        //     font-size: 20px;
                        // }
                        // button{
                        //     background-color: #20AD96;
                        //     color: white;
                        //     padding: 10px 20px;
                        //     border:none;
                        //     font-size: 18px;
                        // }
                    }
                    // .col-2{
                        
                    // }
                }
            }
    }
</style>