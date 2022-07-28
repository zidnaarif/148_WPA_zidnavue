<template>
    <div class="services-card">
        <div class="circle-icon position-relative mx-auto">
            <img :src="`${image}`" alt="" class="position-absolute top-50 start-50 translate-middle">
        </div>
        <h3 class="mt-4">{{title}}</h3>
        <p class="mt-2">Sample text. Click to select the text box. Click again or double click to start editing the text.</p>
    </div>
</template>

<script>
export default {
        props: ['title', 'image']
    }
</script>