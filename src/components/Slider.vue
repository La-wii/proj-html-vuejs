<template>
    <div class="slider">
        <div class="container-lg">
            <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active btn-slider" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
                </div>
            <div class="carousel-inner">
                    <div class="carousel-item active">
                        <!-- <img src="..." class="d-block w-100" alt="..."> -->
                        <div class="row py-5">
                            <div class="col-4" v-for="(testimonial, index) in testimonials" :key="index">
                                <div class="card d-block w-100">
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
                        </div>
                    </div>
                    <div class="carousel-item">
                        <!-- <img src="..." class="d-block w-100" alt="..."> -->
                        <div class="row py-5">
                            <div class="col-4" v-for="(testimonial, index) in testimonials" :key="index">
                                <div class="card d-block w-100 bg-info" style="width: 18rem;">
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
                        </div>
                    </div>
                    <div class="carousel-item">
                        <!-- <img src="..." class="d-block w-100" alt="..."> -->
                        <div class="row py-5">
                            <div class="col-4" v-for="(testimonial, index) in testimonials" :key="index">
                                <div class="card d-block w-100 bg-dark">
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
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev btn-slider" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next btn-slider" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Header",
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
          text: 'I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to be adopted for learners of all levels.',
          img: '/img/testimonial-avata-04.jpg',
          nome:'Luvic Dubble',
          position:'/ Private Tutor'
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
    .slider{
        height: 800px;
        .container-lg{
            .btn-slider{
                color: turquoise;
            }
        }
    }
</style>