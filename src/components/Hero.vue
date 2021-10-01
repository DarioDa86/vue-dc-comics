<template>
    <div class="hero-container" :style="`background-image : url(${bgImage})`">
    </div>
</template>

<script>
export default {
    name: 'Hero',
    props: [
        'bgImage'
    ]

}
</script>

<style>

.hero-container {
    width: 100%;
    height: 350px;
    background-repeat: no-repeat;
    background-size: cover;
}

</style>