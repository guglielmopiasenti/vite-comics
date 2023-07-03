<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],

        }
    }
}
</script>
<template>
    <div class="container">
        <div class="header">
            <img src="src/assets/img/dc-logo.png" alt="DC logo">
            <ul>
                <li v-for="link in links" :class="{ active: link.current }">{{ link.text }}</li>
            </ul>
        </div>
    </div>
</template>

<!-- Header style -->
<style lang="scss" scoped>
@use 'src/assets/scss/_var.scss' as *;

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}

img {
    height: 60px;
}

ul {
    display: flex;
    gap: 15px;
    list-style-type: none;
    text-transform: uppercase;
    font-size: 13px;
    font-weight: 800;
    color: #666768;
}

.active {
    color: $blue;
    position: relative;
}

.active::after {
    content: "";
    position: absolute;
    bottom: -41px;
    left: 0;
    width: 100%;
    height: 5px;
    background-color: $blue;
}
</style>