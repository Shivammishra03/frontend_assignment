<template>
    <div class="new-product-main-outer-sec">
        <div class="new-product-sec" v-for="(tshirt, index) in newTshirtData" :key="index">
            <div class="product-img-sec">
                <img :src="tshirt.productImage" alt="">
            </div>
            <div class="product-detail">{{ tshirt.productName }}</div>
            <div class="product-prize">₹{{tshirt.price}} <s class="strick-text">₹{{tshirt.oldPrice}}</s></div>
            <div class="product-size-sec">
                <div class="small" v-for="size in tshirt.sizes" :key="size">{{ size }}</div>
            </div>
        </div>
    </div>
    <div class="view-all-btn">
        <button class="view-all-btn-text">VIEW ALL</button>
    </div>
</template>

<script>
    export default {
        name:'NewProducts',
        data() {
            return {
                newTshirtData:[
                    {
                        productImage: require('@/assets/images/trending-tshirt-1.svg'),
                        productName: 'Men Henley Neck Full Sleeve Red Wine',
                        price: 399,
                        oldPrice: 1299,
                        sizes: ['S','M','L','XL','XXL']
                    },
                    {
                        productImage: require('@/assets/images/trending-tshirt-2.svg'),
                        productName: 'Men Henley Neck Full Sleeve Red Wine',
                        price: 399,
                        oldPrice: 1299,
                        sizes: ['S','M','L','XL','XXL']
                    },
                    {
                        productImage: require('@/assets/images/trending-tshirt-3.svg'),
                        productName: 'Men Henley Neck Full Sleeve Red Wine',
                        price: 399,
                        oldPrice: 1299,
                        sizes: ['S','M','L','XL','XXL']
                    },
                    {
                        productImage: require('@/assets/images/trending-tshirt-4.svg'),
                        productName: 'Men Henley Neck Full Sleeve Red Wine',
                        price: 399,
                        oldPrice: 1299,
                        sizes: ['S','M','L','XL','XXL']
                    },
                ] 
            }
        }
    }
</script>

<style lang="scss" scoped>
.new-product-main-outer-sec {
    grid-template-columns: repeat(4, 1fr);
    display: grid;
    -moz-column-gap: 16px;
    column-gap: 16px;
    row-gap: 32px;
    .new-product-sec {
        position: relative;
        display: flex;
        flex-direction: column;
        .strick-text {
            color: #FF0000;
        }
        .product-size-sec {
            display: flex;
            align-items: center;
            justify-content: center;
            .small {
                border: 1px solid #E6E6E6;
                /* width: 36px; */
                /* height: 36px; */
                padding: 8px;
                margin-right: 8px;
            }
        }
    }
}
.view-all-btn {
    padding-top: 45px;
    button {
        width: 170px;
        height: 48px;
        background: #770015;
        color: #fff;
        border: none;
        cursor: pointer;
    }
}
</style>