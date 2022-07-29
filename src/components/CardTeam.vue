<template>
    <div class="profileimg">
        <img :src="`${image}`" alt="">
    </div>
    <h5>{{name}}</h5>
    <span>{{tittle}}</span>
</template>

<script>
export default {
    props: ['image', 'name', 'tittle']
}
</script>