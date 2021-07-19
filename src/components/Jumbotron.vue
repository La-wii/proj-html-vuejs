<template>
    <div class="jumbotron">
        <!-- start container -->
        <div class="container-lg">
            <!-- start row -->
            <div class="row">
                <!-- start text section -->
                <div class="col-6 p-5">
                    <h1 class="display-3 my-5">
                        <strong>
                            Distant learning for further expansion
                        </strong>    
                    </h1>

                    <p class="my-3">
                        Learning is a life-long journey that in fact we never find the terminate stop. Stop searching, enjoy the process.
                    </p>

                    <button class="my-3 btn-green">
                        <i class="fas fa-download px-1"></i>
                        Download free guide
                    </button>

                    <p class="my-3">
                        Have questions?
                        <a href="#" class="green">Get Free Sample
                            <i class="fas fa-arrow-right"></i>
                        </a>
                    </p>
                </div>
                <!-- end text section -->

                <!-- start img section -->
                <div class="col-6 py-5 position-relative">
                    <img src="/img/jumbo-img.jpg" alt="" class="rounded-circle">

                    <img src="/img/pallini-grigi.png" alt="pallini" class="gr-dot">

                    <img src="/img/pallini-verdi.png" alt="pallini verdi sfondo" class="green-dot">

                    <img src="/img/cerchio.png" alt="pallini verdi sfondo" class="circle">
                </div>
                <!-- end img section -->
            </div>
            <!-- end row -->

            <div class="row pb-5">
                <div class="col-2">
                    <img src="/img/client-logo-01.png" alt="logo stylus" class="ps-4 pt-1">
                </div>
                <div class="col-2">
                    <img src="/img/client-logo-02.png" alt="logo tree" class="ps-2">
                </div>
                <div class="col-2">
                    <img src="/img/client-logo-03.png" alt="logo brook" class="pt-3">
                </div>
                <div class="col-2">
                    <img src="/img/client-logo-04.png" alt="logo pencil" class="pt-3">
                </div>
                <div class="col-2">
                    <img src="/img/client-logo-05.png" alt="logo it's alive" class="pt-3">
                </div>
                <div class="col-2">
                    <img src="/img/client-logo-07.png" alt="logo nowhere" class="pt-1">
                </div>
            </div>
        </div>
        <!-- end container -->
    </div>
</template>

<script>
export default {
    name: "Jumbotron",
}
</script>

<style scoped lang="scss">
    .jumbotron{
        background-color: #efefef;
        margin-top: -50px;
        .container-lg{
            // start row
            .row{
                // start text
                .col-6{
                    h1{
                        color: #48495f;
                    }
                    p{
                        color: #9ea4a5;
                        font-size: 22px;
                    }
                    p{
                        .green{
                            color: #25ab94;
                        }
                    }
                }
                // start img
                .col-6{
                    .gr-dot{
                        width: 250px;
                        position: absolute;
                        left: -5%;
                        bottom: 50%;
                        z-index: -10;
                    }
                    .green-dot{
                        width: 200px;
                        position: absolute;
                        left: 60%;
                        bottom: 10%;
                        z-index: -10;

                    }
                    .circle{
                        position: absolute;
                        left: 80%;
                        bottom: 50%;
                        z-index: 10;
                    }

                }
            }
            // end row
        }
    }
</style>