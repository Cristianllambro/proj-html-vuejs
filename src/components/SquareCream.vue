<template>
    <div class="container">
        <div class="square">
            <div class="img-sq">
                <img src="../../public/img/shaving_butter-400x400.png" alt="">
            </div>
            <div class="txt-sq">
                <p class="txt">THIS MONTHS FEATURED PRODUCTS</p>
                <h2>Shaving Butter</h2>
                <p class="txt-small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium exercitationem deserunt nobis voluptates optio dolor accusamus. Dignissimos cupiditate iure quo vero dolorum suscipit itaque repellendus quis ipsum tempora, non porro.</p>
                <button class="btn-shop">BUY NOW</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SquareCream',
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container{
    width: 100%;
    height: 50vh;
    position: relative;
    
    .square{
        width: 1000px;
        margin: 0 auto;
        display: flex;
        border-top: 4px solid $light_gold;
        position: absolute;
        top: -5%;
        left: 25%;
        transform: -50%;

        .img-sq{
            width: 40%;
            height: 400px;
            background-image: url(../../public/img/avadabarbers-cta-background.jpg);
            background-size: cover;
            background-repeat: no-repeat;
        }

        .txt-sq{
            padding-left: 2.5rem;
            padding-top: 2.5rem;
            background-color: $cod_gray;
            .txt{
                color: $light_gold;
                margin-bottom: .6rem;
            }
            h2{
                color: $silver;
                font-size: 40px;
                margin-bottom: 1.7rem;
            }
            .txt-small{
                font-size: 15px;
                line-height: 25px;
                color: $silver;
            }
            .btn-shop{
                color: $light_gold;
                padding: .8rem 2rem;
                background-color: transparent;
                border: 2px solid $light_gold;
                cursor: pointer;
                margin-top: 1rem;

                &:hover{
                    transform: scale(1.1);
                }
                
            }
        }
    }
}
</style>