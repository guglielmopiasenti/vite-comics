<script>
import AppComicCard from './AppComicCard.vue';
import AppJumbotron from './AppJumbotron.vue';
import AppButton from './AppButton.vue';
export default {
    components: { AppComicCard, AppJumbotron, AppButton },
    props: { comicBooks: Array }
}
</script>
<template>
    <section id="main">
        <h1 class="title">CURRENT SERIES</h1>
        <AppJumbotron />
        <div class="container">
            <AppComicCard :comicBooks="comicBooks" />
            <AppButton />
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use 'src/assets/scss/_var.scss' as *;

#main {
    background-color: #1C1C1C;
    position: relative;
    z-index: 0;
}

.title {
    position: absolute;
    top: 35%;
    left: 16%;
    transform: translate(-50%, -50%);
    background-color: $blue;
    color: white;
    padding: 10px 20px;
    font-size: 20px;
    font-weight: bold;
    z-index: 1;
}
</style>