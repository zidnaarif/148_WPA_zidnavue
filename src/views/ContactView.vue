<template>

    <ContactVue/>

</template>

<script>
import ContactVue from '@/components/ContactVue.vue'

export default {
    setup() {
    },
    mounted() {
        document.title = "Contact";
    },
    components: {
        ContactVue
    }
}
</script>