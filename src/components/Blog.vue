<template>
    <div class="blog py-5">
        <div class="container-lg py-5">
            <div class="row">

                <div class="col-4">
                    <p class="pb-3">ENJOYABLE INSIGHTS</p>
                    <h2 class="pb-3">Most Viewed<span> Best Blogs</span></h2>

                    <ul>
                        <li class="pb-3">
                            <a href="#">
                                <i class="fas fa-arrow-right"></i>
                                Become a Better Blogger: Content Planning
                            </a>
                        </li>
                        <li class="pb-3">
                            <a href="#">
                                <i class="fas fa-arrow-right"></i>
                                Promoting Your Online Business on Pinterest
                            </a>
                        </li>

                        <li class="pb-3">
                            <a href="#">
                                <i class="fas fa-arrow-right"></i>
                                Gamification and Game-Based Learning
                            </a>
                        </li>

                        <li class="pb-3">
                            <a href="#">
                                <i class="fas fa-arrow-right"></i>
                                Designing an Online Course from Expert’s Perspective
                            </a>
                        </li>
                        
                        <li class="pb-3">
                            <a href="#">
                                <i class="fas fa-arrow-right"></i>
                                Why Online Courses Are the Future of Education
                            </a>
                        </li>

                    </ul>
                    
                    
                </div>

                <div class="col-4">
                    <div class="card" style="width: 25rem;">
                        <img src="/img/blog-1.jpeg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="card-text">
                              BUSINESS  
                            </p>
                            <h5 class="card-title">
                                Ten Benefits Of Rentals That May Change Your Perspective
                            </h5>
                            <span>
                                <i class="far fa-calendar-alt"></i>
                                Dec 28, 2020
                            </span>
                            <span>
                                <i class="far fa-eye"></i>
                                1,231 views
                            </span>
                            
                        </div>
                    </div>
                </div>

                <div class="col-4">
                    <div class="card" style="width: 25rem;">
                        <img src="/img/blog-2.jpeg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="card-text">
                                BUSINESS  
                            </p> 
                            <h5 class="card-title">
                                10 Things Successful Mompreneurs Do Different
                            </h5>
                            <span>
                                <i class="far fa-calendar-alt"></i>
                                Dec 28, 2020
                            </span>
                            <span>
                                <i class="far fa-eye"></i>
                                1,188 views
                            </span>
                                                       
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Blog",
}
</script>

<style scoped lang="scss">
    .blog{
        background-color: #f5f1ed;
        .container-lg{
            .row{
                .col-4{
                    h2{
                        font-weight: bold;
                        span{
                            color: #20AD96;
                        }
                    }
                    ul{
                        li{
                            list-style: none;
                            // margin: bottom;
                            a{
                                font-size: 14px;
                                margin-left: -30px;
                            }
                        }
                    }
                    
                }
                .col-4{
                    .card{
                        border: none;
                        p{
                        font-size: 18px;
                        }
                        h5{
                            font-size: 25px;
                        }
                        span{
                            margin-right: 20px;
                        }
                    }
                }
            }
        }
    }
</style>