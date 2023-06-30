<script>
export default {
    props: {
        comicBooks: Array
    }
}
</script>
<template>
    <ul>
        <li v-for="comic in comicBooks" :key="comic.series">
            <img :src="comic.thumb" :alt="comic.series">
            {{ comic.series }}
        </li>
    </ul>
</template>
<style></style>