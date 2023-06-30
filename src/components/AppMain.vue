<script>
import AppComicCard from './AppComicCard.vue';

export default {
    components: { AppComicCard },
    props: { comicBooks: Array }
}
</script>
<template>
    <section id="main">

        <div class="container">
            <AppComicCard :comicBooks="comicBooks" />
        </div>
    </section>
</template>

<style lang="scss" scoped>
#main {
    background-color: #1C1C1C;
}
</style>