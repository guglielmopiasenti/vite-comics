<script>
import AppComicCard from './components/AppComicCard.vue'

export default {
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

ul {
    padding: 30px 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;

    li {
        width: calc(100% / 6);
        padding: 20px 20px;
        color: white;
        font-size: smaller;


        img {
            display: block;
            height: 150px;
            width: 150px;
            object-fit: cover;
            background-position: top;
            margin-bottom: 20px;
        }
    }
}
</style>