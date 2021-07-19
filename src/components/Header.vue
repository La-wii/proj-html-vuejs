<template>
<header>

    <nav>
        <!-- start container -->
        <div class="container-lg">
            <!-- start row -->
            <div class="row py-2">
                <!-- start logo -->
                <div class="col-2 pt-3">
                    <img src="/img/dark-logo.png" alt="logo" class="logo">
                </div>
                <!-- end logo -->

                <!-- start link -->
                <div class="col-8 pt-4 d-inline-flex">
                    <ul>
                        <li v-for="(link, index) in link" :key="index" class="px-4"> 
                            <a :href="link.url">{{link.text}}</a>
                            
                            <!-- <ul>
                                <li v-for="(page, index) in pages" :key="index" >
                                    <a :href="page.url">{{page.text}}</a>
                                </li>
                                                           
                            </ul> -->

                            <!-- <ul>
                                <li><a href="#"></a>a</li>
                                <li><a href="#"></a>b</li>
                                <li><a href="#"></a>c</li> 
                            </ul> -->
                        </li>


                    </ul>

                    <!-- <ul>
                        <li v-for="(page, index) in pages" :key="index" >
                            <a :href="page.url">{{page.text}}</a>
                        </li>
                                                           
                    </ul> -->

                    <div class="icon mx-3">
                        <i class="far fa-user-circle"></i>
                    </div>
                </div>
                <!-- end link -->
                
                <!-- start input -->
                <div class="col-2 d-inline-flex">

                    <input type="text" 
                        class="form-control" 
                        placeholder="Search"
                        v-model.trim="inputText"
                    >

                    <button type="submit" 
                    class="ms-2 px-2"
                    >
                        <i class="fas fa-search lente"></i>
                    </button>               

                </div>
                <!-- end input -->
            </div>
            <!-- end row -->
        </div>
        <!-- end container -->
    </nav>

</header>

</template>

<script>
export default {
    name: "Header",
    data (){
    return {
        link :[
        {
          text: 'Home',
          url:'#',
          current: false
        },
        {
          text: 'Pages',
          url:'#',
          current: false
        },
        {
          text: 'Courses',
          url:'#',
          current: false
        },
        {
          text: 'Features',
          url:'#',
          current: false
        },
        {
          text: 'Blog',
          url:'#',
          current: false
        },
        {
          text: 'Shop',
          url:'#',
          current: false
        }
        ],
        pages:[
        {
          text: 'link 1',
          url:'#',
          current: false
        },
        {
          text: 'link 2',
          url:'#',
          current: false
        },
        {
          text: 'link 3',
          url:'#',
          current: false
        }
        ]
    }
  }
}
</script>

<style scoped lang="scss">
    header{
        nav{
            // position: relative;
            .container-lg{
                .row{
                    .col-2{
                        .logo{
                            width: 150px;
                            height: 35px;
                        }
                    }
                    .col-8{
                        ul{
                            li{
                                display: inline-block;
                                list-style: none;
                                font-size: 14px;
                                    // ul{
                                    //     li{
                                    //         display: block;
                                    //         display: none;               
                                    //             &:hover{
                                    //                 display: block;
                                    //             }
                                    //         a{
                                    //            color: transparent;
                                    //             li:hover a{
                                    //                color: black;
                                    //             }
                                    //         }


                                            
                                    //     }
                                    // }
                            }
                        }
                        .icon{
                            &:hover{
                                color: #20AD96;
                            }
                        }
                    }
                    .col-2{
                        button{
                            .lente:hover{
                                color: #20AD96;
                            }
                        }
                    }
                }
            }
        }
    }
</style>