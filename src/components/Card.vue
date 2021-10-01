<template>
    <div class="card">
        <img class="comics__image" :src="card.thumb" :alt="card.thumb">
        <div class="text__image">
            {{card.series}}
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['card']

}
</script>

<style lang="scss" scoped>
    .card {
        width: 15%;
        height: 150px;
        border: 1px solid #fff;
        margin: 30px 5px;

        .comics__image {
            width: 100%;
        }
    }

</style>