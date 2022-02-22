<template>
    
    <div class="slider">
        
        <div class="box-slider">
            <h2 class="title">Slider prodotti</h2>
            <ul class="ul-slider">

                <li class="li-product" v-for="(product, index) in products" :key="index">
                    <img class="img-product" :src=product.src alt="">
                    <span class="exclusive">{{product.esclusiva}}</span>
                    <h4 class="name-product">{{product.nameProduct}}</h4>
                    <span class="description-cost">{{product.description}}</span>
                    <span class="description-cost">{{product.cost}}</span>
                </li>   

                <i class="fab fa-medium"></i>

            </ul>
        </div>
    </div>

</template>

<script>
export default{
    name: 'mySlider',
    props: {
        msg: String
    },

    data () {

        return {

            products : [

                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
                {
                    src: require('../assets/img/scarpa-blazer-low-77-jumbo-kZsBBt.jpg'),
                    esclusiva: 'Esclusiva',
                    nameProduct: 'Nome Prodotto',
                    description: 'Descrizione prodotto',
                    cost: '0.00 $'
                },
            ]
        }


    }
}

    
</script>

<style>
    @import "../assets/style/general.scss";

    /* Slider */
    .box-slider {
        width: 92%;
        margin: auto;
        margin-bottom: 50px;
        margin-top: 20px;
    } 

    .ul-slider {
        width: 1295px;
        height: 610px;
        margin-top: 20px;
        display: flex;
        flex-direction: row;
        overflow-x: scroll;
    }

    .li-product {
        list-style: none;
        display: flex;
        flex-direction: column;
        height: 100%;
        width: 34%;
        padding: 0px 5px;
    }

    .exclusive {
        line-height: 26px;
        color: #ff0017;
        font-size: 18px;
        font-weight: 400;
        line-height: 28px;
        margin-top: 15px;
    }

    .name-product {
        font-size: 18px;
        font-weight: 400;
        line-height: 26px;
    }

    .description-cost {
        font-size: 16px;
        font-weight: 400;
        line-height: 28px;
        color: #757575;
    }
    /* Slider */
</style>