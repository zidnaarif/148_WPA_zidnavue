<template>
  <NavbarVue/>
  <HeroVue/>

  <section id="service">
    <div class="container">
        <div class="row mt-4">
          <div class="col-12 text-center">
            <h2>Our Services</h2>
            <span class="subtitle">We design & deliver beautiful hotels, luxury homes and innovative workplace interiors.</span>
          </div>
        </div>

        <div class="row mt-5">
          <div class="col-md-3 text-center">
            <ServiceVue title="Projects" :image="'assets/img/icons8-ratings-96.png'"/>
          </div>
          <div class="col-md-3 text-center">
            <ServiceVue title="Great Design" :image="'assets/img/icons8-armchair-96.png'"/>
          </div>
          <div class="col-md-3 text-center">
            <ServiceVue title="Home Decor" :image="'assets/img/icons8-curtains-96.png'"/>
          </div>
          <div class="col-md-3 text-center">
            <ServiceVue title="About us" :image="'assets/img/icons8-trust-96.png'"/>
          </div>
        </div>
    </div>
  </section>

  <SearchVue/>

  <section id="ourdesign">
    <div class="container-fluid mb-5">
      <div class="container position-relative">
          <div class="position-absolute top-50 start-0">
            <h2>Our Design</h2>
          </div>
          <div class="position-absolute top-50 end-0 mt-3">
            <button class="button-secondary rounded-pill">More ></button>
          </div>
      </div>
    </div>

    <div class="row container-fluid">
        <div class="container mt-5 subtittle text-center mx-auto">
          <span>We design & deliver beautiful hotels, luxury homes and innovative workplace interiors. 
            Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem.</span>
        </div>
    </div>

    <div class="container mt-2 mb-2">
      <div class="ms-5 me-5">
        <CardDesign/>
      </div>
    </div>
  
  </section>

  <ReviewVue/>

  <ContactVue/>
  <FooterVue/>
</template>

<script>
// @ is an alias to /src
import NavbarVue from '../components/NavbarVue.vue'
import HeroVue from '../components/HeroVue.vue'
import ServiceVue from '../components/ServiceVue.vue'
import SearchVue from '../components/SearchVue.vue'
import FooterVue from '../components/FooterVue.vue'
import ContactVue from '../components/ContactVue.vue'
import ReviewVue from '../components/ReviewVue.vue'
import CardDesign from '@/components/CardDesign.vue'

export default {
  name: 'HomeView',
  data() {
    return {
      web_name : "Dekoruma"
    }
  },
  components: {
    NavbarVue,
    HeroVue,
    ServiceVue,
    SearchVue,
    FooterVue,
    ContactVue,
    CardDesign,
    ReviewVue
}
}
</script>
