<template>
    <div class="cta-section">
        <!-- start container -->
        <div class="container-lg">
            <div class="row">
                <!-- start col -->
                <div class="col-3">
                    
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-6 text-center">
                    <h2>Start today for getting <span>Online Certification</span></h2>
                    <p>You can be your own guiding star with our help!</p>
                    <button>
                        Get started now
                    </button>
                </div>
                <!-- end col -->

                <!-- start col -->
                <div class="col-3">

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
                    .col-3{

                    }
                    .col-6{
                        h2{
                            span{
                                color: #20AD96;
                            }
                        }
                        p{
                            font-size: 20px;
                        }
                        button{
                            background-color: #20AD96;
                            color: white;
                            padding: 10px 20px;
                            border:none;
                            font-size: 18px;
                        }
                    }
                    .col-3{
                        
                    }
                }
            }
    }
</style>