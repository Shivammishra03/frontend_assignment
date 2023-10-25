<template>
    <div class="main-outer-offer-section">
        <div class="offers-section-1">
            <img src="@/assets/images/offer-1.svg" alt="">
            <img src="@/assets/images/offer-2.svg" alt="">
        </div>
        <div class="offer-section-2">
            <img src="@/assets/images/offer-3.svg" alt="">
            <img src="@/assets/images/offer-4.svg" alt="">
            <img src="@/assets/images/offer-5.svg" alt="">
        </div>
    </div>
</template>

<script>
    export default {
        name: "OfferSection",
    }
</script>

<style lang="scss" scoped>
.main-outer-offer-section {
    .offers-section-1 {
        display: flex;
        align-items: center;
        justify-content: space-around;
        margin-bottom: 16px;
    }
    .offer-section-2 {
        display: flex;
        align-items: center;
        justify-content: space-around;
        margin-bottom: 16px;
    }
}
</style>