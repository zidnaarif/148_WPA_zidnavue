<template>

    <div id="galleryview">
        <GalleryVue/>
    </div>

</template>

<script>
import GalleryVue from '@/components/GalleryVue.vue';

export default {
    data() {
        return {
            web_name: "Dekoruma"
        };
    },

    components: {
        GalleryVue
    }
}
</script>
