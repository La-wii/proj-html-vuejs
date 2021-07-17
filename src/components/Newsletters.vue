<template>
    <div class="newsletters-content py-5">
        <div class="container-lg py-5">
            <!-- start row -->
            <div class="row py-5">
                <!-- start col -->
                <div class="col-12 text-center position-relative">
                       
                    <h2 class="text-capitalize display-6">subscribe 
                        <span class="text-capitalize">newsletter</span> 
                    </h2>

                    <p>
                        Enter your email address to register to our newsletter subscription
                        <br>
                        delivered on a regular basis!
                    </p>

                    <img src="/img/pallini-grigi-obliqui.png" alt="pallini" class="dots">

                    <img src="/img/cerchio.png" alt="cerchio" class="cerchio">
                </div>
                <!-- end col -->
            </div>
            <!-- end row -->

            <!-- start row -->
            <div class="row text-center">
                <!-- start col -->
                <div class="col-3">
                    
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-6 d-inline-flex">
                    
                    <input type="text" 
                        class="form-control" 
                        placeholder="Enter your email"
                        v-model.trim="inputText"
                    >

                    <button type="submit" 
                    class="ms-2 px-2 btn-green">Subscribe</button>        
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-3">
                    
                </div>
                <!-- end col -->
            </div>
            <!-- end row -->
        </div>
    </div>
</template>

<script>
export default {
    name: "Youtube",
}
</script>

<style scoped lang="scss">
    .newsletters-content{
        
        .container-lg{
            .row{
                .dots{
                    position: absolute;
                    right: -5%;
                    bottom: 0;
                }
                .cerchio{
                    width: 100px;
                    position: absolute;
                    right: -5%;
                    bottom: 0;
                }
                h2{
                    span{
                        color: #20AD96;
                    }
                }
                p{
                    font-size: 25px;
                    color: #2c3837;
                }
            }

            .row{
                input{
                    height: 60px;
                }
            }
        }
    }
</style>