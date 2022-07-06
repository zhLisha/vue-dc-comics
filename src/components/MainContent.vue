<template>
    <div class="main-content">
        <div class="container">
        <span> --  Content goes here -- </span>
    </div>
    </div>
</template>

<script>
export default {
    name: 'MainContent'
}
</script>

<style lang="scss" scoped>
@import '../common/variables';

.main-content {
    background-color: $secondColor;
    color: $mainFontColor;
    height: 80px;

    span {
        font-size: 20px;
        line-height: 80px;
    }
}
</style>