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
                        <li v-for="(link, index) in link" :key="index"> 
                            <a :href="link.url">{{link.text}}</a>
                            <div class="col-2">
                                <ul v-if="link.subitems"> 
                                    <li v-for="(page, index) in link.subitems" :key="index" >
                                        <a class="dropdown" :href="page.url">
                                            {{page.text}}
                                        </a>
                                    </li>
                                </ul>                            
                            </div>    
                        </li>
                    </ul>


                    <div class="icon">
                        <i class="far fa-user-circle"></i>
                    </div>
                </div>
                <!-- end link -->
                
                <!-- start input -->
                <div class="col-2 d-inline-flex pt-3">

                    <input type="text" 
                        class="form-control" 
                        placeholder="Search"
                        v-model.trim="inputText"
                    >

                    <button type="submit" 
                    class="ms-2"
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
          current: false,
            subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,          
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
        },
        {
          text: 'Pages',
          url:'#',
          current: false,
            subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
        },
        {
          text: 'Link',
          url:'#',
          current: false,
          subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,
          
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
        },
        {
          text: 'Features',
          url:'#',
          current: false,
          subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,
          
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
        },
        {
          text: 'Blog',
          url:'#',
          current: false,
          subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,
          
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
        },
        {
          text: 'Shop',
          url:'#',
          current: false,
          subitems:[
            {
            text: 'Link',
            url:'#',
            current: false,
          
            },
            {
            text: 'Link',
            url:'#',
            current: false
            },
            {
            text: 'Link',
            url:'#',
            current: false
            }              
            ]
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
                            height: 30px;
                            object-fit: cover;
                        }
                    }
                    .col-8{
                        ul{
                            margin-left: 30px;
                            li{
                                display: inline-block;
                                list-style: none;
                                font-size: 14px;    
                                    &:hover .dropdown{
                                            color: black;
                                           
                                    }
                                    ul{
                                        padding: 0;
                                        li{
                                            .dropdown{
                                                
                                                color: transparent;
                                                // padding-left: -20px;
                                                // margin-right: -30px;
                                                &:hover{
                                                    color: #20AD96;
                                                    
                                                }
                                            }                                           
                                        }
                                    }
                            }
                        }
                        .icon{
                            &:hover{
                                color: #20AD96;
                            }
                        }
                    }
                    .col-2{
                        height: 60px;
                        input{
                            background-color: #efefef;
                            border: none;
                            margin-right: -10px;
                        }
                        button{
                            border: none;
                            width: 50px;
                            // margin-left: 0px;
                            .lente{
                                color: #20AD96;
                            }
                        }
                    }
                }
            }
        }
    }
</style>