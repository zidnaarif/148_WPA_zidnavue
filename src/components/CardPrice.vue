<template>
    <div class="price-card text-center">
        <div class="circle-icon position-relative mx-auto">
            <img :src="`${image}`" alt="" class="position-absolute top-50 start-50 translate-middle">
        </div>
            <p>{{plan}}</p>
            <h2>{{price}}</h2>
            <h3 class="mt-4">{{title}}</h3>
            <li>Lorem Ipsum</li>
            <li>Dolor Sitema</li>
            <li>Sed ut perspiciatis</li>
            <li>Magni Dolores</li>
            <li>Nemo Enim</li>
            <li>Eiusmod Tempor</li>
        <div>
            <button class="btn-submit rounded-pill mt-3">Choose plan</button>
        </div>
    </div>
</template>

<script>
export default {
    props: ['plan', 'image', 'price', 'title']
}
</script>
