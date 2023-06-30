<script>
import AppComicCard from './AppComicCard.vue';
import AppJumbotron from './AppJumbotron.vue';

export default {
    components: { AppComicCard, AppJumbotron },
    props: { comicBooks: Array }
}
</script>
<template>
    <section id="main">
        <AppJumbotron />
        <div class="container">
            <AppComicCard :comicBooks="comicBooks" />
            <button>LOAD MORE</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use 'src/assets/scss/_var.scss' as *;

#main {
    background-color: #1C1C1C;
}

button {
    padding: 5px 25px;
    color: white;
    background-color: $blue;
    border-color: $blue;
}
</style>