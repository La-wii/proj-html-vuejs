<template>
    <div class="counter">
        <div class="container-lg">
            <div class="row">

                <div class="col-3">
                    <div class="card text-center p-5">
                        <div class="card-body">
                            <h5 class="card-title">
                                Successfully
                                <br>
                                trained
                            </h5>
                            <p class="card-text green">
                                1790
                            </p>
                            <p class="card-text">
                                ENROLLED LEARNERS
                            </p>  
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card text-center p-5">
                        <div class="card-body">
                            <h5 class="card-title">
                                Proudly
                                <br>
                                Received
                            </h5>
                            <p class="card-text green">
                                19
                            </p>
                            <p class="card-text">
                                COUNTRYWIDE AWARDS
                            </p>  
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card text-center p-5">
                        <div class="card-body">
                            <h5 class="card-title">
                                Firmly
                                <br>
                                Established
                            </h5>
                            <p class="card-text green">
                                24
                            </p>
                            <p class="card-text">
                                LOCAL BRANCHES
                            </p>  
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="card text-center p-5">
                        <div class="card-body">
                            <h5 class="card-title">
                                Getting
                                <br>
                                Featured on
                            </h5>
                            <p class="card-text green">
                                1090
                            </p>
                            <p class="card-text">
                                BLOG POSTS
                            </p>  
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Count",
}
</script>

<style scoped lang="scss">
    .counter{
        .container-lg{
            .row{
                .col-3{
                    .card{
                        height: 300px;
                        .card-body{
                            // .card-title{

                            // }
                            .green{
                                color: #20AD96;
                                font-size: 50px;
                                font-weight: bold;
                            }
                        }
                    }
                }
            }
        }
    }
</style>