<template>
    <div class="main-content">
       <div class="container">
            <!-- Current Series -->
            <div class="current-series btn">
                <span> CURRENT SERIES </span>
            </div>

            <ul class="series-list flex">
                <SeriesCard v-for="(card, index) in allSeriesList" :key="index" :cardDetails="card" />
            </ul>

            <!-- Load More BTN -->
            <button class="btn">
                <span>LOAD MORE</span>
            </button>
       </div>
    </div>
</template>

<script>
import SeriesCard from './SeriesCard.vue'
import arraySeries from '../assets/dc-comics.json'

export default {
    name: 'SeriesList',
    components: {
        SeriesCard
    },

    data() {
        return {
            allSeriesList: arraySeries
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../common/variables';

.main-content {
    background-color: $secondColor;
    color: $mainFontColor;

    .container {
        text-align: center;
        position: relative;
    }

    .series-list {
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 35px 0;
        position: relative;
        text-align: left;
    }

    .current-series {
        position: absolute;
        padding: 10px 25px;
        font-size: 20px;
        top: -23px;
        left: -20px;
    }

    .btn {
        background-color: $mainColor;
        border: none;
        color: $mainFontColor;
        font-weight: 700;
    }

   button {
        padding: 10px 50px;
        font-size: 12px;
        margin-bottom: 30px;
        cursor: pointer;
    }
}
</style>