<template>

    <NavbarVue/>

    <div id="galleryview">
        <GalleryVue/>
    </div>

    <FooterVue/>

</template>

<script>
import NavbarVue from '../components/NavbarVue.vue';
import FooterVue from '../components/FooterVue.vue';
import GalleryVue from '../components/GalleryVue.vue';

export default {
    data() {
        return {
            web_name: "Dekoruma"
        };
    },

    components: {
    NavbarVue,
    GalleryVue,
    FooterVue
}
}
</script>
