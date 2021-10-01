<template>
    <div class="card">
        <div class="card-img-box">
            <img class="comics__image" :src="card.thumb" :alt="card.thumb">
        </div>
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
        margin: 20px 0;

        .card-img-box {
            width: 80%;
            padding-bottom: 80%;
            margin: 1em auto;
            overflow: hidden;
            position: relative;

            .comics__image {
                position: absolute;
                width: 100%;
            }
        }

        .text__image {
            margin:  0 0 0 10% ;
        }
    }

</style>