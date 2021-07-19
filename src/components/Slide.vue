<template>
    <div class="box">

        <div class="slider-box">
            <div class="row">
                <div class="col-12 text-center">
                    <p class="py-2">GREAT WORDS ABOUT MAXCOACH</p>
                    <h2 class="display-6">Our<span> top learners' </span>verbatim</h2>
                </div>
            </div>
            <div class="row py-5">
                <VueSlickCarousel :arrows="false" :dots="true" :slidesToShow="3">
                   <div class="col-4" v-for="(testimonial, index) in testimonials" :key="index">
                    <div class="card mx-3">
                        <div class="card-body">
                            <h5 class="card-title">{{testimonial.title}}</h5>
                            <p class="card-text">{{testimonial.text}}</p>
                            <!-- <a href="#" class="btn btn-primary">Button</a> -->
                            <p>{{testimonial.nome}}</p>
                            <img :src="testimonial.img" alt="" class="card-img rounded-pill">
                            <span class="card-text">
                                <small class="text-muted pe-5">
                                {{testimonial.position}}
                                </small>
                            </span>
                        </div>
                    </div>
                </div> 
                
                </VueSlickCarousel>
                
            </div>
        </div>
    
    </div>  
</template>

<script>

  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name: "Slide",
    components: { VueSlickCarousel },
    data (){
    return {
      testimonials :[
        {
          title: 'High level of efficiency and scientific teaching methods',
          text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
          img: '/img/testimonial-avata-02.jpg',
          nome:'Mina Hollace',
          position:'/Freelancer'
        },
        {
          title: 'Professional team of specialists and passionate mentors at reach ',
          text: 'I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.',
          img: '/img/testimonial-avata-03.jpg',
          nome:'John Blabla',
          position:'/ IT Specialist'
        },
        {
          title: 'The MaxCoach team works really hard to ensure high quality',
          text: 'I am happy with their arrangement of lessons and subjects. They reflect a scientific investigation into effective methods to be adopted for learners of all levels.',
          img: '/img/testimonial-avata-04.jpg',
          nome:'Luvic Dubble',
          position:'/ Private Tutor'
        },
        {
          title: 'High level of efficiency and scientific teaching methods',
          text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
          img: '/img/testimonial-avata-02.jpg',
          nome:'Mina Hollace',
          position:'/Freelancer'
        },
        {
          title: 'Professional team of specialists and passionate mentors at reach ',
          text: 'I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.',
          img: '/img/testimonial-avata-03.jpg',
          nome:'John Blabla',
          position:'/ IT Specialist'
        },
        {
          title: 'The MaxCoach team works really hard to ensure high quality',
          text: 'I am happy with their arrangement of lessons and subjects. They reflect a scientific investigation into effective methods to be adopted for learners of all levels.',
          img: '/img/testimonial-avata-04.jpg',
          nome:'Luvic Dubble',
          position:'/ Private Tutor'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
    .box{
        background-color: #f6f3f5;
        // height: 800px;
        .slider-box{
            .row{
                .col-12{
                    p{
                    color: #9ea4a5;
                    }
                    span{
                        color:#20AD96;
                    }
                }
            }
            .row{
                .col-4{
                    .card{
                        height: 400px;
                        border: none;
                        .card-body{
                            .card-img{
                                width: 30px;
                                height: 30px;
                            }
                        }
                    }
                }
            }
        }
    }
</style>