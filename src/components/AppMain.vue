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
        <AppJumbotron />
        <div class="container">
            <AppComicCard :comicBooks="comicBooks" />
            <AppButton />
        </div>
    </section>
</template>

<style lang="scss" scoped>
#main {
    background-color: #1C1C1C;
}
</style>