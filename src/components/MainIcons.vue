<template>
    <div class="main-icons">
        <ul class="small-container flex">
            <li v-for="(icons, index) in mainIcons" :key="index">
                <a href="icons.url" class="flex">
                    <div class="icon">
                        <img :src="icons.icon">
                    </div>
                    <div class="icon-name">
                        {{icons.text}}
                    </div>
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'MainIcons',
    data() {
        return {
            mainIcons: [
                {
                    text: 'DIGITAL COMICS',
                    url:  '#',
                    icon: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    text: 'DC MERCHANDISE',
                    url:  '#',
                    icon: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    text: 'SUBSCRIPTION',
                    url:  '#',
                    icon: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url:  '#',
                    icon: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'DC POWER VISA',
                    url:  '#',
                    icon: require('../assets/img/buy-dc-power-visa.svg')
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../common/variables';

.main-icons {
    height: 100px;
    background-color: $mainColor;
    color: $mainFontColor;

    .small-container {
        height: 100%;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    img {
        width: 35px;
    }

    .icon-name {
        font-size: 11px;
        font-weight: 300;
        padding-left: 10px;
    }
    a {
        align-items: center;
    }
}
</style>
