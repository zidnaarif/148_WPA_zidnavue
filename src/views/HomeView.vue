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

  <section id="ourdesign" class="overflow-hidden">
    <div class="container">
      <div class="row">
        <div class="col-md-9">
          <h2>Our Design</h2>
        </div>
        <div class="col-md-3 my-auto">
          <button class="button-secondary rounded-pill">More ></button>
        </div>
      </div>
    </div>

    <div class="row mt-5 container mx-5">
      <div class="container-fluid">
        <div class="col-12 subtittle text-center">
          <span>We design & deliver beautiful hotels, luxury homes and innovative workplace interiors. 
            Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem.</span>
        </div>
      </div>
    </div>

    <div class="container position-relative">
      <div class="row mt-5">
        <div class="owl-carousel owl-theme">
          <div class="item mb-4">
            <CardDesign :image="'assets/img/brown-living-room.jpg'" title="Living Room" desc="Model A-11"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/green-living.jpg'" title="Living Room" desc="Model A-13"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/kitchen-studio.jpg'" title="Kitchen" desc="Model B-11"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/luxury-bedroom.jpg'" title="Bed Room" desc="Model C-22"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/brown-living-room.jpg'" title="Living Room" desc="Model A-18"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/green-living.jpg'" title="Living Room" desc="Model A-12"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/kitchen-studio.jpg'" title="Kitchen" desc="Model B-11"/>
          </div>

          <div class="item mb-4">
            <CardDesign :image="'assets/img/luxury-bedroom.jpg'" title="Bed Room" desc="Model C-22"/>
          </div>
          
        </div>
      </div>
    </div>
  </section>

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
import CardDesign from '../components/CardDesign.vue'

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
    CardDesign
}
}
</script>
