<template>
    <div class="main-header-secrion">
        <div class="header-sec-1">
            <div class="header-txt-1">Welcome to Our Store Hiscraves</div>
            <div class="header-contact-sec">
                <img src="@/assets/images/phone-icon.svg" alt="">
                <div class="contact-text">Call Us: 1234567890</div>
            </div>
        </div>
        <div class="header-sec-2">
            <div class="menu-icon-sec">
                <img src="@/assets/images/menu-icon.svg" alt="">
            </div>
            <div class="logo-section">
                <div class="logo-text">Logo Here</div>
            </div>
            <div class="user-detail-section">
                <img src="@/assets/images/search-icon.svg" class="search-icon" alt="" >
                <img src="@/assets/images/wishlist-icon.svg" class="wishlist-icon" alt="">
                <img src="@/assets/images/add-product-detail-icon.svg" class="add-product-detail-icon" alt="">
                <img src="@/assets/images/userdetail-icon.svg" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderSection'
        
    }
</script>

<style lang="scss" scoped>
.main-header-secrion {
    .header-sec-1 {
        background-color: #1F1F1F;
        padding-top: 14.7px;
        padding-bottom: 14.7px;
        display: flex;
        align-items: center;
        justify-content: space-around;
        .header-txt-1 {
            color: #FFF;
        }
        .header-contact-sec {
            display: flex;
            align-items: center;
            .contact-text {
                color: #FFF;
                margin-left: 8px;
            }
        }
    }
    .header-sec-2 {
        box-shadow: 0px 8px 21px 0px #00000029;
        background-color: #FFFFFF;
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        padding-top: 30px;
        padding-bottom: 30px;
        .user-detail-section {
            display: flex;
            align-items: center;
            .wishlist-icon {
                margin-left: 16px;
                margin-right: 16px;
            }
            .add-product-detail-icon {
                margin-right: 16px;
            }
        }
    }
}

</style>