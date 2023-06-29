<script>
export default {
    data() {
        return {
            links: [
                {
                    img: 'src/assets/img/buy-comics-digital-comics.png',
                    title: 'DIGITAL COMICS',
                },
                {
                    img: 'src/assets/img/buy-comics-merchandise.png',
                    title: 'DC MERCHANDISE',
                },
                {
                    img: 'src/assets/img/buy-comics-subscriptions.png',
                    title: 'SUBSCRIPTION',
                },
                {
                    img: 'src/assets/img/buy-comics-shop-locator.png',
                    title: 'COMIC SHOP LOCATOR',
                },
                {
                    img: 'src/assets/img/buy-dc-power-visa.svg',
                    title: 'DC POWER VISA',
                },
            ],
        }
    }
}
</script>

<template>
    <section id="upper-footer">
        <div class="container">
            <ul class="upper-footer-list">
                <li v-for="link in links"> {{ link.img }} {{ link.title }}</li>
            </ul>
        </div>
    </section>
    <section id="main-footer">
        <div class="container">
            <div class="list-container">
                <div>
                    <ul class="m-footer-list">
                        <li>
                            <h4>DC COMICS</h4>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <ul class="m-footer-list">
                        <li>
                            <h4>SHOP</h4>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collections</li>
                    </ul>
                </div>
                <ul class="m-footer-list">
                    <li>
                        <h4>DC</h4>
                    </li>
                    <li>Terms Of Use</li>
                    <li>Privacy Policy (new)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshop</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
                <ul class="m-footer-list">
                    <li>
                        <h4>SITES</h4>
                    </li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>
    </section>
    <section id="lower-footer">
        <div class="container"></div>
    </section>
</template>

<style scoped>
#upper-footer {
    background-color: #0782F9;
    padding: 30px 0;
}

.upper-footer-list {
    display: flex;
    color: white;
}

/*  */
#main-footer {
    background-image: url(src/assets/img/footer-bg.jpg);
    padding: 30px 0;
}

.list-container {
    display: flex;
    gap: 20px;
}

.m-footer-list>li {
    color: grey;
}

h4 {
    color: white;
}

.list-container>li {
    color: grey;
}

#lower-footer {
    background-color: #303030;
}
</style>