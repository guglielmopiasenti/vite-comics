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
        <div class="container"></div>
    </section>
    <section id="main-footer">
        <div class="container"></div>
    </section>
    <section id="lower-footer">
        <div class="container"></div>
    </section>
</template>

<style>
#upper-footer {
    background-color: #0782F9;
}

#main-footer {}

#lower-footer {
    background-color: #303030;
}
</style>