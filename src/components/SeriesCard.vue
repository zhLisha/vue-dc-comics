<template>
        <li class="card"> 
            <img :src="cardDetails.thumb" :alt="cardDetails.type">
            <div class="thumb-title">
                <span>{{cardDetails.series}}</span>
            </div>
        </li>
</template>


<script>
export default {
    name: 'SeriesCard',
    props: {
        cardDetails: Object
    }
}
</script>

<style lang="scss" scoped>
.card {
    margin:20px 10px;
    width: calc((100% / 5) - 20px);

    // img {
    //     // height: 150px;
    //     object-fit: cover;
    //     overflow: hidden;
    //     object-position: top;
    // }

    .thumb-title {
        font-size: 12px;
    }
}
</style>