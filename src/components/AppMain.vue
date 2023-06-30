<script>
export default {
    props: { comicBooks: Array }
}
</script>
<template>
    <section id="main">
        <div class="container">
            <ul>
                <li v-for="comic in comicBooks" :key="comic.series">
                    <img src="comic.thumb" alt="comic.series">
                    {{ comic.series }}
                </li>
            </ul>
        </div>
    </section>
</template>
<style scoped>
#main {
    background-color: #1C1C1C;
}

h2 {
    color: white;
    padding: 60px 0;
    text-align: center;
}
</style>