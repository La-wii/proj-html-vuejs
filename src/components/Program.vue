<template>
    <!-- start program -->
    <div class="program py-5">

        <!-- start container-lg -->
        <div class="container-lg">
            
            <!-- start col -->
            <div class="col-12 py-5">
            
            <!-- start row -->
            <div class="row">

                <div class="top text-center py-3">
                    <p class="text-uppercase">
                        max coach available                        
                    </p>
                    <h2 class="text-capitalize display-6">access 
                        <span class="text-capitalize">smart tutoring</span> 
                        program for benefits
                    </h2>
                </div>

                <div class="card" style="width: 22rem;">
                    <img src="/img/custom.png" class="card-img-top pb-4" alt="Preferences">
                    <div class="card-body">
                        <h5 class="card-title h4 pt-3">Customize Preferences</h5>
                        <p class="card-text">Learners are given the right to arrange and customize their study schedule and timetable based on preferences.</p>
                        <a href="#">
                            Start here
                            <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>    

                <div class="card" style="width: 22rem;">
                    <img src="/img/cloud-storage.png" class="card-img-top pb-4" alt="Cloud Storage">
                    <div class="card-body">
                        <h5 class="card-title h4 pt-3">Cloud Storage</h5>
                        <p class="card-text">You can store online lessons via online cloud or download to your device and revise lessons on the way.
                        </p>
                        <a href="#">
                            Get Free Quote
                            <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>


                <div class="card" style="width: 22rem;">

                    <img src="/img/multimedia.png" class="card-img-top" alt="Multimedia">
                    <div class="card-body">
                        <h5 class="card-title h4">Multimedia Channels</h5>
                        <p class="card-text">We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.</p>
                        <a href="#">
                            Start now
                            <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>

                </div>

            </div>
            <!-- end row -->

            </div>
            <!-- end col -->
        </div>
        <!-- end container-lg -->
    </div>
    <!-- end program -->
</template>

<script>
export default {
    name: "Program",
}
</script>

<style scoped lang="scss">
    .program{
        .container-lg{
            .col-12{
                .top{
                    p{
                        color: #9ea4a5;
                        font-size: 18px;
                    }
                    h2{
                        color: #48495f;
                        span{
                            color: #20AD96;
                        }
                    }
                }
                .card{
                    width: calc(100% / 3);
                    border: none;
                    margin: 35px;
                    h5{
                        color: #48495f;
                    }
                    p{
                        color: #9ea4a5;
                    }
                }
            }
        }
    }
</style>