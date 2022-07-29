<template>

  <NavbarVue/>

  <section id="about" class="overflow-hidden">
    <div class="container">
      <div class="container-fluid about mt-5 mb-5 text-center">
        <div class="row">
          <div class="col-12">
            <h3>Our mission is to make beautiful interior design for everyone.</h3>
            <span>Start Bootstrap was built on the idea that quality, functional website templates and themes should be available to everyone. Use our open source, free products, or support us by purchasing one of our premium products or services.</span>
            <div class="mt-5 mb-2">
              <button class="button-secondary rounded-pill">Our Story ></button>
            </div>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="aboutcard d-lg-flex align-items-center mx-auto">
          <div class="col-md-6 mx-auto my-auto">
            <div class="imgcard">
              <img src="/assets/img/luxury-living-room-mockup.jpg"/>
            </div>
          </div>
  
          <div class="col-md-6 mx-auto my-auto">
            <span>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</span>
          </div>
        </div>
      </div>

      <div class="row mt-5">
        <div class="col-12 mb-5 text-center team">
          <h3>Our team</h3>
          <span>Dedicated to quality and your success.</span> 
        </div>
        
        <div class="teamcard d-lg-flex mx-auto align-items-center">
          <div class="col-md-3 text-center">
            <CardTeam name="Sarah Earlen" tittle="CEO" :image="'/assets/img/employee3.jpg'" />
          </div>

          <div class="col-md-3 text-center">
            <CardTeam name="Rachel Madeline" tittle="CFO" :image="'/assets/img/employee4.jpg'" />
          </div>

          <div class="col-md-3 text-center">
            <CardTeam name="Gabriel Daan" tittle="Operations Manager" :image="'/assets/img/employee1.jpg'" />
          </div>

          <div class="col-md-3 text-center">
            <CardTeam name="Kevin Oakley" tittle="CTO" :image="'assets/img/employee2.jpg'" />
          </div>
        </div>

      </div>

      <div class="container-fluid about mt-5 text-center">
        <div class="row mt-5">
          <div class="col-12 mt-5">
            <p>This website created by Muh. Zidna Arif A. as a mini-project for completing
            Web Programming online course by Work in Tech INCO Academy & Alterra Academy using Vue JS Framework and Bootstrap 5.2.
            </p> 
            <div class="mt-5 mb-2">
              <button class="button-secondary rounded-pill">My Portfolio</button>
            </div>
          </div>
        </div>
      </div>
      
    </div>
  </section>

  <FooterVue/>

</template>

<script>
import NavbarVue from '@/components/NavbarVue.vue'
import FooterVue from '@/components/FooterVue.vue'
import CardTeam from '@/components/CardTeam.vue'

export default {
    setup() {
    },
    mounted() {
      document.title = "About us";
    },
    components: {
    NavbarVue,
    FooterVue,
    CardTeam
  }
}
</script>
