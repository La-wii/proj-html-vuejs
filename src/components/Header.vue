<template>
<header>

    <nav>
        <!-- start container -->
        <div class="container-lg">
            <!-- start row -->
            <div class="row py-2">
                <!-- start logo -->
                <div class="col-2 py-1">
                    <img src="/img/dark-logo.png" alt="logo" class="logo">
                </div>
                <!-- end logo -->

                <!-- start link -->
                <div class="col-7 d-inline-flex pt-3">
                    <ul>
                        <li v-for="(link, index) in link" :key="index"> 
                            <a :href="link.url" class="mx-3">{{link.text}}</a>
                            <!-- <ul>
                                <li v-for="(page, index) in pages" :key="index" >
                                    <a :href="page.url">{{page.text}}</a>
                                </li>
                            </ul> -->
                        </li>
                    </ul>

                    <div class="icon mx-3">
                        <i class="far fa-user-circle"></i>
                    </div>
                </div>
                <!-- end link -->
                
                <!-- start input -->
                <div class="col-3 d-inline-flex">

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
            .container-lg{
                .row{
                    .col-2{
                        .logo{
                            width: 180px;
                            height: 45px;
                        }
                    }
                    .col-7{
                        ul{
                            li{
                                display: inline-block;
                                list-style: none;
                                font-size: 20px;
                                    // ul{
                                    //     li{
                                    //         display: block;
                                    //         display: none;
                                    //             &:hover li{
                                    //             display: block;
                                    //             }
                                            
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
                    .col-3{
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