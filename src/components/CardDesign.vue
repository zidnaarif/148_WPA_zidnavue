<template>
    <div class="card border-0 shadow">
        <img :src="`/${image}`" alt="" class="card-img-top">
        <div class="card-body">
            <h4>{{title}}</h4>
            <span>{{desc}}</span>
        </div>
    </div>
</template>

<script>
export default {
        props: ['title', 'image', 'desc']
    }
</script>
