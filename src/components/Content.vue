<template>
    <div class="content-container pb-5">
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
                <div class="col-12 mx-0 my-3 promo-container">
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

        <div class="row mx-0 justify-content-center pb-3 pt-5 title-content">
            Our Products
        </div>
        <div class="row col-12 justify-content-center mx-0" >
            <div class="row col-11 mx-0 justify-content-center px-0 product-container">
                <div class="col-12 mx-0 mt-4 py-2 pl-4 header-article">
                    Featured Product
                </div>
                <div class="col-4 mx- 0">
                    <img class="object-fit_contain" src="../assets/images/product1.png">
                    <p class="py-2 mx-5 title-article">GENSET OSSEL RX7500</p>
                </div>
                <div class="col-4 mx-0 object-fit_contain">
                    <img class="object-fit_contain" src="../assets/images/product1.png">
                    <p class="py-2 mx-5 title-article">GENSET OSSEL RX7500</p>
                </div>
                <div class="col-4 mx-0 object-fit_contain">
                    <img class="object-fit_contain" src="../assets/images/product1.png">
                    <p class="py-2 mx-5 title-article">GENSET OSSEL RX7500</p>
                </div>
                <div class="col-12 mx-0 mt-4 py-2 pl-4 header-article">
                    Latest Product
                </div>
                <div class="col-4 mx- 0">
                    <img class="object-fit_contain" src="../assets/images/product2.jpg">
                    <p class="py-2 mx-5 title-article">JIGSAW P-431</p>
                </div>
                <div class="col-4 mx-0 object-fit_contain">
                    <img class="object-fit_contain" src="../assets/images/product2.jpg">
                    <p class="py-2 mx-5 title-article">JIGSAW P-431</p>
                </div>
                <div class="col-4 mx-0 object-fit_contain">
                    <img class="object-fit_contain" src="../assets/images/product2.jpg">
                    <p class="py-2 mx-5 title-article">JIGSAW P-431</p>
                </div>
            </div>
        </div>

        <div class="row mx-0 justify-content-center pt-3 pb-5 mt-5  title-content about-us-container">
            About Us
        </div>
        <div class="row col-12 mx-0 about-us-container justify-content-center">
            <div class="row col-8 pb-4" style="text-align:center;">
                OSSEL adalah sebuah merk terdaftar untuk mesin dan alat-alat teknik untuk mendukung pekerjaan dan kegiatan produksi. Produk-produk OSSEL telah memenuhi standard kualitas dan sertifikasi International yang mencakup bidang : Pertukangan Dan Perbengkelan, Power Tools/ Mesin Perkakas, General Machinery, Pertanian Dan Perkebunan, Food Machinery Dan Packaging. OSSEL hadir untuk memenuhi kebutuhan masyarakat Indonesia akan mesin dan alat-alat teknik dengan standard kualitas International dan harga yang terjangkau. Semua produk-produk OSSEL bisa didapat di hampir seluruh Toko-Toko Teknik dan online market di Indonesia.
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