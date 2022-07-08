<template>
        <li class="card"> 
           <a href="#">
                <div class="image">
                    <img :src="cardDetails.thumb" :alt="cardDetails.type">
                </div>
                <div class="thumb-title">
                    <span>{{cardDetails.series}}</span>
                </div>
           </a>
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
    margin:20px 0;
    width: calc((100% / 6) - 20px);

    .image {
        object-fit: cover;
        overflow: hidden;
      object-position: top;
        margin-bottom: 15px;
        aspect-ratio: 1/1;
    }

    .thumb-title {
        font-size: 11.5px;

        span {
            text-transform: uppercase;
            font-weight: 300;
        }
    }
}
</style>