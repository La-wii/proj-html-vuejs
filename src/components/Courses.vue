<template>
  <!-- start corsi -->
  <div class="corsi py-5">
    <!-- start container -->
    <div class="container-lg">
      <div class="row">
        <div class="col-12 text-center pb-5">
          <p>STIMULATED TO LEARN?</p>
          <h2 class="display-6">
            <strong>
                Featured Online Courses
            </strong>
            </h2>
        </div>
      </div>

      <div class="row">
        <div class="col-6" v-for="(corso, index) in corsi" :key="index">

          <div class="card mb-3" style="width: 40rem;">

            <div class="row g-0">

              <div class="col-md-4 pt-2">
                <img :src="corso.img" class="img-fluid rounded-circle" alt="immagini">
              </div>

              <div class="col-md-8">
                <div class="card-body">
                  <h5 class="card-title">{{corso.prezzo}}</h5>
                  <p class="card-text">{{corso.descrizione}}</p>
                  <span class="card-text">
                    <small class="text-muted pe-5">
                      <i class="far fa-file"></i>
                      {{corso.lezioni}} Lessons
                    </small>

                    <small class="text-muted">
                      <i class="far fa-user"></i>
                      {{corso.studenti}}
                    </small>
                  </span>
                </div>
              </div>

            </div>

          </div>

        </div>
      </div>

    </div>
    <!-- start container -->
  </div>
  <!-- end corsi -->
</template>

<script>
export default {
  name: "Courses",
  data(){
   return{
      corsi:[
        {
          img: '/img/corso-1.jpg',
          costo:'Free',
          descrizione: 'Personal Finance: Financial Security Thinking & Principles',
          lezioni: '2',
          studenti: '95',
          alt: 'Thinking & Principles',
        },
        {
          img: '/img/corso-2.jpg',
          costo:'$40,00',
          descrizione: 'Learning to Write as a Professional Author',
          lezioni: '20',
          studenti: '50',
          alt: 'Write as a Professional Author',
        },
        {
          img: '/img/corso-3.jpg',
          costo:'Free',
          descrizione: 'Customer-centric Info-Tech Strategies',
          lezioni: '24',
          studenti: '821',
          alt: 'Info-Tech Strategies',
        },
        {
          img: '/img/corso-4.jpg',
          costo:'$19,00',
          descrizione: 'Open Programming Courses for Everyone: Python',
          lezioni: '17',
          studenti: '62',
          alt: 'Python',
        },
        {
          img: '/img/corso-6.jpg',
          costo:'$26,00',
          descrizione: 'Academic Listening and Note-taking',
          lezioni: '14',
          studenti: '67',
          alt: 'Academic Listening',
        },
        {
          img: '/img/corso-6.jpg',
          costo:'$39,00',
          descrizione: 'Master jQuery in a Short Period of Time',
          lezioni: '6',
          studenti: '51',
          alt: 'Master jQuery',
        },
      ]
    }
  }
  
}
</script>

<style scoped lang="scss">
  .corsi{
    background-color: #f6f3f5;
      .container-lg{
        .row{
          .col-12{
            p{
              color: #9ea4a5;
            }
          }
        }
        .row{
          .card{
            height: 150px;
            width: calc(100% / 2);
            // margin: 10px;
            background-color: transparent;
            border: none;
              .card-img{
                height: 150px;
                width: 150px;
                border-radius: 50%;
              }
            }
        }
      }
  }
    

    
</style>