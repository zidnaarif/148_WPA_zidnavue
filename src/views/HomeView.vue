<template>
  <NavbarVue/>
  <HeroVue/>

</template>

<script>
// @ is an alias to /src
import NavbarVue from '../components/NavbarVue.vue'
import HeroVue from '../components/HeroVue.vue'

export default {
  name: 'HomeView',
  data() {
    return {
      web_name : "Dekoruma"
    }
  },
  components: {
    NavbarVue,
    HeroVue
}
}
</script>
