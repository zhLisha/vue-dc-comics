<template>
    <div class="jumbotron-bg">
       <div class="container">
            <!-- Image Logo -->
            <!-- <img src="../assets/img/dc-logo-bg.png" alt="Footer Jumbo Logo"> -->

            <!-- Content List -->
            <div class="content-list flex">

                <!-- Left column list -->
                <ul class="footer-list">
                    <li class="list-container flex">
                        <ul class="dc-comics-list">
                            <li v-for="(elementList, index) in footerListLeft" :key="index">
                                <!-- Title -->
                                <div class="title">
                                    {{ elementList.title }}
                                </div>

                                <ul>
                                    <li v-for="(elementA, index) in footerListLeft[index].listA" :key="index">
                                        <a  href="elementList.url">
                                            {{ elementA.link }}
                                        </a>
                                    </li>
                                </ul>
                            </li>
                        </ul>

                        <ul class="dc-general-list">
                            <li v-for="(elementList, index) in footerListGeneral" :key="index">
                                <!-- Title -->
                                <div class="title">
                                    {{ elementList.title }}
                                </div>

                                <ul>
                                    <li v-for="(elementA, index) in footerListGeneral[index].listA" :key="index">
                                        <a  href="elementList.url">
                                            {{ elementA.link }}
                                        </a>
                                    </li>
                                </ul>
                            </li>
                        </ul>

                        <ul class="shop-list">
                            <li v-for="(elementList, index) in footerListSites" :key="index">
                                <!-- Title -->
                                <div class="title">
                                    {{ elementList.title }}
                                </div>

                                <ul>
                                    <li v-for="(elementA, index) in footerListSites[index].listA" :key="index">
                                        <a  href="elementList.url">
                                            {{ elementA.link }}
                                        </a>
                                    </li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
       </div>
    </div>
</template>

<script>
export default {
    name: 'FooterJumbo',
    data() {
        return {
            footerListLeft: [
                {
                    title: 'DC COMICS',
                    url: '#',
                    listA: [
                        {
                            link: 'Charactera'
                        },
                        {
                            link: 'Comics'
                        },
                          {
                            link: 'Movies'
                        },
                          {
                            link: 'TV'
                        },
                          {
                            link: 'Games'
                        },
                          {
                            link: 'VideosS'
                        },
                          {
                            link: 'News'
                        }
                    ]   
                },
                {
                    title: 'SHOP',
                    url: '#',
                    listA: [
                        {
                            link: 'Shop DC'
                        },
                        {
                            link: 'Shop DC COllectibles'
                        }
                    ]   
                }
            ],
            footerListGeneral: [
                {
                    title: 'DC',
                    url: '#',
                    listA: [
                        {
                            link: 'Terms Of Use'
                        },
                        {
                            link: 'Privacy policy (New)'
                        },
                        {
                            link: 'Ad Choices'
                        },
                        {
                            link: 'Advertasing'
                        },
                        {
                            link: 'Jobs'
                        },
                        {
                            link: 'Subsciptions'
                        },
                        {
                            link: 'Talent Workshops'
                        },
                        {
                            link: 'CPSC Certificates'
                        },
                        {
                            link: 'Ratings'
                        },
                        {
                            link: 'Shop Help'
                        },
                        {
                            link: 'Contact Us'
                        }
                    ]   
                }
            ],
            footerListSites: [
                {
                    title: 'SITES',
                    url: '#',
                    listA: [
                        {
                            link: 'DC'
                        },
                        {
                            link: 'MAD Magazine'
                        },
                         {
                            link: 'Dc Kids'
                        },
                        {
                            link: 'DC Universe'
                        },
                        {
                            link: 'DC Power Visa'
                        }
                    ]   
                }
            ] 
        }
    }
}

</script>

<style lang="scss" scoped>
@import '../common/variables';

.jumbotron-bg {
    height: 350px;
    background-image: url('../assets/img/footer-bg.jpg');
    position: relative;
    color: white;

    .container {
        height: 100%;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
    }

    // img {
    //     width: 500px;
    //     position: absolute;
    //     bottom: -60px;
    //     right: 150px;
       
    // }
}

.footer-list {
    a {
        font-size: 11px;
        font-weight: 300;
        color: $footerFontColor;
    }
}

.content-list {
    height: 100%;
    display: flex;
    align-items: center;

    .title {
        padding-top: 20px;
        padding-bottom: 5px;
    }
}

.list-container {
    ul {
        padding-right: 20px;
    }
}

</style>