<template>
    <div class="header">
        <div class="container flex">
            <!-- Logo -->
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="Dc Logo">
            </div>
            <!-- Nav -->
            <nav>
                <ul class="flex">
                    <li v-for="(list, index) in navList" :key="index" :class="{'current': list.current}">
                        <a href="list.url"> {{ list.text }} </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderDc',
    data() {
        return {
            navList: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                 {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                 {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                 {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                 {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                 {
                    text: 'COLLECTIONS',
                    url: '#',
                    current: false
                },
                 {
                    text: 'VIDEO',
                    url: '#',
                    current: false
                },
                 {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                 {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                 {
                    text: 'SHOP',
                    url: '#',
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../common/variables';

.header {
    height: 100px;

    img {
        width: 60px;
        display: inline-block;
        padding-top: 8px;
    }

    .container {
        justify-content: space-between;
        align-items: center;
        height: 100%;
    }
}

ul {
    font-size: 11px;

    li {
        padding:0 10px;
    }

    .current {
    color: $mainColor;
    }

    .current::after {
        content: "";
        border-bottom: 4px solid $mainColor;
        margin: 0 auto;
        display: block;
    }
}


</style>