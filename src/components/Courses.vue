<template>
  <!-- start corsi -->
  <div class="corsi">

    <div class="container-lg">

      <div class="row flex-wrap">

        <div class="col-6">

          <div class="card mb-3">

            <div class="row g-0">

              <div class="col-md-4 corso-img pt-3">
                <img src="/img/corso-1.jpg" class="img-fluid rounded-circle" alt="...">
              </div>

              <!-- start col -->
              <div class="col-md-8">

                <div class="card-body">
                  <h5 class="card-title">Price</h5>
                  <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                  <span class="card-text">
                    <small class="text-muted pe-5">
                      <i class="far fa-file"></i>
                      Lessons
                    </small>

                    <small class="text-muted">
                      <i class="far fa-user"></i>
                      Students
                    </small>
                  </span>
                </div>

              </div>
              <!-- end col -->
            </div>

          </div>

        </div>

      </div>

    </div>

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
          studenti: '95'
        },
        {
          img: '/img/corso-2.jpg',
          costo:'$40,00',
          descrizione: 'Learning to Write as a Professional Author',
          lezioni: '20',
          studenti: '50'
        },
        {
          img: '/img/corso-3.jpg',
          costo:'Free',
          descrizione: 'Customer-centric Info-Tech Strategies',
          lezioni: '24',
          studenti: '821'
        },
        {
          img: '/img/corso-4.jpg',
          costo:'$19,00',
          descrizione: 'Open Programming Courses for Everyone: Python',
          lezioni: '17',
          studenti: '62'
        },
        {
          img: '/img/corso-5.jpg',
          costo:'$26,00',
          descrizione: 'Academic Listening and Note-taking',
          lezioni: '14',
          studenti: '67'
        },
        {
          img: '/img/corso-6.jpg',
          costo:'$39,00',
          descrizione: 'Master jQuery in a Short Period of Time',
          lezioni: '6',
          studenti: '51'
        },
      ]
    }
  }
  
}
</script>

<style scoped lang="scss">
    // .card{
    //   .card-img{
        
    //   }
    // }
</style>