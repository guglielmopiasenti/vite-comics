<script>
export default {

    props: { comicBooks: Array }
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

<style lang="scss" scoped>
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
        text-transform: uppercase;


        img {
            display: block;
            height: 200px;
            width: 200px;
            object-fit: cover;
            object-position: top;
            margin-bottom: 20px;
        }
    }
}
</style>