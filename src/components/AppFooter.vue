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
                <li v-for="link in links" :key="link.title">
                    <img :src="link.img" :alt="link.title" />
                    {{ link.title }}
                </li>
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
        <div class="container">
            <div class="btn-footer">SIGN-UP NOW!</div>
            <div class="footer-logo">
                <h4> FOLLOW US</h4>
                <img src="src/assets/img/footer-facebook.png" alt="Facebook">
                <img src="src/assets/img/footer-twitter.png" alt="Twitter">
                <img src="src/assets/img/footer-youtube.png" alt="YouTube">
                <img src="src/assets/img/footer-pinterest.png" alt="Pinterest">
                <img src="src/assets/img/footer-periscope.png" alt="Periscope">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use 'src/assets/scss/_var.scss' as *;

#upper-footer {
    background-color: $blue;
    padding: 30px 0;
}

.upper-footer-list {
    display: flex;
    justify-content: center;
    gap: 20px;
    color: white;

    li {
        display: flex;
        align-items: center;
        gap: 10px;
        font-size: smaller;
    }

    img {
        height: 40px;
    }
}


/*  */
#main-footer {
    background-image: url(src/assets/img/dc-logo-bg.png), url(src/assets/img/footer-bg.jpg);
    background-position: 75% 50%, center;
    background-size: auto, cover;
    background-repeat: no-repeat;
    padding: 30px 0;
}

.list-container {
    display: flex;
    gap: 20px;
}

.m-footer-list>li {
    color: grey;
    font-size: smaller;
    padding: 3px 0;

    h4 {
        color: white;
        font-size: larger;
        padding: 10px 0;
    }
}



#lower-footer {
    background-color: #303030;
    padding: 30px 0;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}


.btn-footer {
    color: white;
    border: 2px solid $blue;
    padding: 15px;
    font-weight: 700;
}

.footer-logo {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;

    h4 {
        color: $blue;
        font-weight: 800;
    }
}
</style>