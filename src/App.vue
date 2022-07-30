<template>

  <NavbarVue/>
  <router-view/>
  <FooterVue/>

</template>

<script>
import NavbarVue from '@/components/NavbarVue.vue';
import FooterVue from '@/components/FooterVue.vue';

export default {
    data() {
        return {
            web_name: "Dekoruma"
        };
    },

    components: {
    NavbarVue,
    FooterVue
  }
}
</script>