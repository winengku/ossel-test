<template>
    <div class="content-container">
        <div class="row mx-0">
            <div class="col-5 product-list-container">
                <div class="pt-5">
                    <div v-for="product in products" :key="product.id"
                    class="product-list-style">
                        <a href="#"> {{product.text}} </a>
                    </div>
                </div>
            </div>
            <div class="row col-7 mx-0 justify-content-center">
                <div class="col-12 mx-0 mt-3 mb-0 promo-container">
                    <div class="col-12 mx-0 px-0 py-2 promo-title">
                        Our Promo
                    </div>
                    <agile :initial-slide="1" :infinite="true" :autoplay="true" :navButtons="false" class="mb-2">
                        <img class="slide" src="../assets/images/promo.jpeg"/>
                        <img class="slide" src="../assets/images/promo.jpeg"/>
                        <img class="slide" src="../assets/images/promo.jpeg"/>
                        <img class="slide" src="../assets/images/promo.jpeg"/>
                    </agile>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { VueAgile } from 'vue-agile'

export default {
    components:{
        agile : VueAgile
    },
    name: 'ProductCategories',
    data() {
        return {
        products: [
            {
            id: 0,
            text: 'PERTUKANGAN & PERBENGKELAN',
            page:'#'
            },
            {
            id: 1,
            text: 'PERTANIAN & PERKEBUNAN',
            page:'#'
            },
            {
            id: 2,
            text: 'GENERAL MACHINERY',
            page:'#'
            },
            {
            id: 3,
            text: 'FOOD MACHINERY & PACKAGING',
            page:'#'
            }
        ]
        }
    }
}
</script>