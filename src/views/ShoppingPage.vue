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
            <TrendingproductionSec/>
        </div>
        <div class="trending-section-outer">
            <div class="trending-heading">
                <!-- <hr/> -->
                Featured Products
            </div>
            <FeaturedProducts/>
        </div>
    </div>
    <div class="banner-sec-2">
        <img src="@/assets/images/banner-2.svg" alt="" />
    </div>
    <div class="middle-section">
        <div class="trending-section-outer">
            <div class="trending-heading">
                <!-- <hr/> -->
                New Products
            </div>
            <NewProducts/>
        </div>
        <div class="trending-section-outer">
            <div class="trending-heading">
                <!-- <hr/> -->
                Best Selling Products
            </div>
            <BestsellingProducts/>
        </div>
    </div> 
</template>

<script>
import HeaderSection from '@/components/HeaderSection.vue';
import OfferSection from '@/components/OfferSection.vue';
import TrendingproductionSec from '@/components/TrendingproductionSec.vue';
import FeaturedProducts from '@/components/FeaturedProducts.vue';
import NewProducts from '@/components/NewProducts.vue';
import BestsellingProducts from '@/components/BestsellingProducts.vue';
    export default {
        name: "ShoppingPage",
        components: {
            HeaderSection,
            OfferSection,
            TrendingproductionSec,
            NewProducts,
            BestsellingProducts,
        }
    }
</script>

<style lang="scss" scoped>
.banner-sec-1 {
    img {
        width: -webkit-fill-available;
    }
}
.banner-sec-2 {
    padding-bottom: 32px;
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
    .trending-section-outer {
        padding-top: 16px;
        padding-bottom: 32px;
        .trending-heading {
            position: relative;
            padding-bottom: 32px;
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
}

</style>