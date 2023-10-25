<template>
    <HeaderSection/>
    <div class="banner-sec-1">
        <img src="@/assets/images/banner-1.svg" alt="" />
    </div>
    <div class="middle-section">
        <div class="product-catogery-section">
            <div class="row">
                <div>
                    <img src="@/assets/images/men-tshirts-img.png" alt="">
                    <label for="">Men’s T-Shirts</label>
                </div>
                <div>
                    <img src="@/assets/images/women-wears-img.png" alt="">
                    <label for="">Women’s Wear</label>
                </div>
                <div>
                    <img src="@/assets/images/winter-collection-img.png" alt="">
                    <label for="">Winter Collections</label>
                </div>
                <div>
                    <img src="@/assets/images/hooded-img.png" alt="">
                    <label for="">Hooded T-Shirts</label>
                </div>
                <div>
                    <img src="@/assets/images/polo-neck-img.png" alt="">
                    <label for="">Polo Neck T-Shirts</label>
                </div>
                <div>
                    <img src="@/assets/images/full-sleeves-img.png" alt="">
                    <label for="">Full Sleeves T-Shirts</label>
                </div>
            </div>
        </div>
        <OfferSection/>
        <div class="trending-section-outer">
            <div class="trending-heading">
                <!-- <hr/> -->
                Trending T-Shirts
            </div>
        </div>
    </div> 
</template>

<script>
import HeaderSection from '@/components/HeaderSection.vue';
import OfferSection from '@/components/OfferSection.vue';
    export default {
        name: "ShoppingPage",
        components: {
            HeaderSection,
            OfferSection
        }
    }
</script>

<style lang="scss" scoped>
.banner-sec-1 {
    img {
        width: -webkit-fill-available;
    }
}
.middle-section {
    max-width: 1136px;
    margin: auto;
    .product-catogery-section {
        padding-top: 45px;
        padding-bottom: 55px;
    }
    .row {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .trending-heading {
        position: relative;
        &::after {
            content: '';
            position: absolute;
            top: 10px;
            bottom: 0;
            width: 380px;
            background-color: #FFC7D1;
            right: 10px;
            height: 2px;
            opacity: 0.5;
        }
        &::before {
            content: '';
            position: absolute;
            top: 10px;
            bottom: 0;
            width: 380px;
            background-color: #FFC7D1;
            left: 10px;
            height: 2px;
            opacity: 0.5;
        }
    }
}

</style>