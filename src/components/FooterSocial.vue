<template>
    <div class="footer-social">
        <div class="container flex">

            <!-- Button -->
            <div class="button">
                <a class="btn" href="icons.url"><span>SINGN-UP NOW!</span></a>
            </div>

            <!-- Social -->
            <div class="social flex">
                <a href="icons.url"> <span class="flex"> FOLLOW US </span></a>
                <!-- icons -->
                <ul class="social-icons flex">
                    <li v-for="(icons, index) in socialIcons" :key="index">
                        <a href="icons.url"> 
                            <img :src="icons.icon" :alt="icons.alt">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterSocial',
    data() {
        return {
            socialIcons: [
                {
                    url: '#'
                },
                {
                    icon: require('../assets/img/footer-facebook.png'),
                    alt: 'Icona Facebook'
                },
                {
                    icon: require('../assets/img/footer-twitter.png'),
                    alt: 'Icona Twitter'
                },
                {
                    icon: require('../assets/img/footer-youtube.png'),
                    alt: 'Icona Youtube'
                },
                {
                    icon: require('../assets/img/footer-pinterest.png'),
                    alt: 'Icona Pinterest'
                },
                {
                    icon: require('../assets/img/footer-periscope.png'),
                    alt: 'Icona periscope'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../common/variables';

.footer-social {
    height: 80px;
    background-color: $footerBgColor;

    .container {
        height: 100%;
        align-items: center;
        justify-content: space-between;
    }

    .btn {
        color: $mainFontColor;
        border: 2px solid $mainColor;
        padding: 10px 15px;
        font-size: 12px;
        display: block;
    }
}

.social {
    span {
        color: $mainColor;
        vertical-align: middle;
        height: 100%;
        align-items: center;
        font-weight: 700;
        font-size: 18px;
    }

    li {
        padding-left: 15px;
    }
}

</style>