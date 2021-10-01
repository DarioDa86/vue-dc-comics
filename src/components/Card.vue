<template>
    <div class="card">
        <img class="comics__image" src="prod.thumb" alt="comics.thumb">
        <div class="text__image">
            {{series}}
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['prod']

}
</script>

<style>
    .card {
        width: 15%;
        height: 150px;
        border: 1px solid #fff;
        margin: 30px 5px;
    }

</style>