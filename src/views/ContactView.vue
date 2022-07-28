<template>

    <NavbarVue/>
    <ContactVue/>
    <FooterVue/>

</template>

<script>
import NavbarVue from '@/components/NavbarVue.vue'
import ContactVue from '@/components/ContactVue.vue'
import FooterVue from '@/components/FooterVue.vue'

export default {
    setup() {
    },
    components: {
    NavbarVue,
    ContactVue,
    FooterVue
}
}
</script>