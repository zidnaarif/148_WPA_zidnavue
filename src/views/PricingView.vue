<template>
    <NavbarVue/>

  <section id="pricing">
    <div class="container">
        <div class="row mt-4">
          <div class="col-12 text-center">
            <h2>Pay as you grow</h2>
            <span class="subtitle">With our no hassle pricing plans.</span>
          </div>
        </div>

        <div class="row mt-5">
          <div class="col-md-4">
            <CardPrice plan="Small" price="$100" title="Great Design" :image="'/assets/img/icons8-flow-chart-96.png'"/>
          </div>
          
          <div class="col-md-4">
            <CardPrice plan="Medium" price="$200" title="Premium Design" :image="'/assets/img/icons8-mind-map-96.png'"/>
          </div>

          <div class="col-md-4">
            <CardPrice plan="Large" price="$300" title="Exclusive Design" :image="'/assets/img/icons8-venn-diagram-96.png'"/>
          </div>
        </div>

        <div class="row mt-5 text-center">
          <div class="col-12">
            <p>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</p>
          </div>
        </div>

    </div>
  </section>

    <FooterVue/>    
</template>

<script>
import NavbarVue from '@/components/NavbarVue.vue'
import FooterVue from '@/components/FooterVue.vue'
import CardPrice from '@/components/CardPrice.vue'

export default {
    setup() {
    },
    components: {
    NavbarVue,
    FooterVue,
    CardPrice
}
}
</script>