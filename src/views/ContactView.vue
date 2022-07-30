<template>
    <div class="contactpage">
        <ContactVue/>
    </div>

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

<style scoped>
    .contactpage {
        margin-top: 50px;
        min-height: auto;
    }
</style>