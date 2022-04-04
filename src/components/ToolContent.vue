<template>
    <div class="container-tools">

        <!-- TITLE SHOP -->
        <div class="title">
            <p>WE HAVE YOU COVERED</p>
            <h2>Avada Grooming Products</h2>
        </div>

        <!-- SHOP TOOLS -->

        <div class="shop">

            <!-- one -->
            <div class="content" v-for="element in arrShopTools" :key="element.id">
                <img :src="element.img" :alt="element.name">
                <h3>{{ element.name }}</h3>
                <p>{{ element.price }}</p>
            </div>
        </div>

        <button class="btn-shop">SHOP OUR PRODUCT RANGE</button>
    </div>
</template>

<script>
import brush from '../../public/img/../../public/img/brush_dark-400x400.png'
import scissors from '../../public/img/scissors-400x400.png'
import hotOil from '../../public/img/hot_oil_dark-400x400.png'
import razor from '../../public/img/straight_razor_dark-400x400.png'
export default {
    name: 'ToolContent',
    data () {
        return {
            arrShopTools: 
            [
                {
                    id: 1,
                    img: brush,
                    name: 'Brush',
                    price: '$15.00'
                },
                {
                    id: 2,
                    img: scissors,
                    name: 'Scissors',
                    price: '$85.00'
                },
                {
                    id: 3,
                    img: hotOil,
                    name: 'Hot Oil',
                    price: '$15.00'
                },
                {
                    id: 4,
                    img: razor,
                    name: 'Straight Razor',
                    price: '$30.00'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container-tools{
    width: 100%;
    height: 90vh;
    text-align: center;
    background-image: url(../../public/img/avadabarbers-reviewsbackground.jpg);
    background-size: contain;

    .title{
        text-align: center;
        padding-top: 3rem;

        p{
            font-size: 14px;
            color: $teak;
        }
    
        h2{
            color: $silver;
            font-size: 55px;
            font-family: 'Abril Fatface', cursive;
            margin-bottom: 1.5rem;
        }
    }

    .shop{
        width: 100%;
        display: flex;
        justify-content: center;
        .content{
            width: calc(100% / 4 - 1rem);
            text-align: center;

            h3{
                color: $teak;
                font-size: 25px;
                margin-bottom: .5rem;
            }

            p{
                font-size: 14px;
                color: $teak;
            }
        }
    }

    .btn-shop{
        color: $teak;
        padding: .8rem 2rem;
        background-color: transparent;
        border: 2px solid $teak;
        cursor: pointer;
        margin-top: 4rem;

        &:hover{
            transform: scale(1.1);
        }
    }
}
</style>