<template>
  <footer>
    <div class="container-lg">
        <!-- start row -->
        <div class="row py-5">
            <!-- start col -->
            <div class="col-6">

                <h3 class="py-3">Address</h3>

                <p>
                    382 NE 191st St # 87394 Miami, FL 33179-3899
                </p>

                <p>
                    +1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)
                </p>

                <p>
                    support@maxcoach.com   
                </p>

                <div class="social">
                    <a href="#">
                        <i class="fab fa-facebook-square"></i>
                    </a>

                    <a href="#">
                        <i class="fab fa-twitter"></i>
                    </a>

                    <a href="#">
                        <i class="fab fa-instagram"></i>
                    </a>

                    <a href="#">
                        <i class="fab fa-linkedin"></i>
                    </a>

                </div>

            </div>
            <!-- end col -->

            <div class="col-3">
                <h4 class="py-3">Explore</h4>
                <ul>
                    <li v-for="(link, index) in explore" :key="index"> <a :href="link.url">{{link.text}}</a></li>
                </ul>
            </div>

            <div class="col-3">
                <h4 class="py-3">Information</h4>
                <ul>
                    <li v-for="(link, index) in information" :key="index"> <a :href="link.url">{{link.text}}</a></li>
                </ul>
            </div>

        </div>
        <!-- end row -->
    </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data (){
    return {
        explore :[
        {
          text: 'Start here',
          url:'#',
          current: false
        },
        {
          text: 'Blog',
          url:'#',
          current: false
        },
        {
          text: 'About us',
          url:'#',
          current: false
        },
        {
          text: 'Success story',
          url:'#',
          current: false
        },
        {
          text: 'Courses',
          url:'#',
          current: false
        },
        {
          text: 'Contact us',
          url:'#',
          current: false
        }
        ],
        information :[
        {
          text: 'Membership',
          url:'#',
          current: false
        },
        {
          text: 'Puchase guide',
          url:'#',
          current: false
        },
        {
          text: 'Privacy policy',
          url:'#',
          current: false
        },
        {
          text: 'Terms of services',
          url:'#',
          current: false
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
    footer{
        background-color: #f6f3f5;
        .container-lg{
            .row{
                .col-6{
                    .social{
                        a{
                            color: #9ea4a5;
                            font-size: 25px;
                            margin-right: 35px;
                                &:hover{
                                    color: #20AD96;
                                }
                        }
                            
                    }
                }
                .col-3{
                    h4{
                        margin-left: 30px;
                    }
                    ul{
                        li{
                            // display: inline-block;
                            list-style: none;
                                a   {
                                    text-decoration: none;
                                    color: #0b0b0b;
                                        &:hover{
                                            color: #20AD96;
                                        }
                                }
                        }
                    }
                }
            }
        }
    }
</style>