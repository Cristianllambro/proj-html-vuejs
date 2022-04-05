<template>
    <div class="container-footer">
        <div class="flex">
            <!-- block 1 -->
            <div class="left">
                <img src="../../public/img/avadabarbers_footer_shop_image-400x312.png" alt="tools for shaving">
                <button class="btn-footer">SHOP OUR RANGE NOW</button>
            </div>

            <!-- block 2 -->
            <div class="center">
                <img src="../../public/img/avadabarbers-logo-x1.png" alt="logo barber">
                <ul>
                    <li>Avada Barbers</li>
                    <li>123 New York Street</li>
                    <li><a href="#!">info@yourwebsite.com</a></li>
                    <li>+1 (555) 555-1212</li>
                </ul>

                <p>FOLLOW US</p>

                <ul class="icons">
                    <li><i class="fa-brands fa-facebook-f"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-youtube"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                </ul>
            </div>

            <!-- block 3 -->
            <div class="right">
                <img src="../../public/img/avadabarbers_footer_appointment_image-400x312.png" alt="img barber">
                <button class="btn-footer">BOOK YOUR APPOINTMENT</button>
            </div>
        </div>

        <div class="foot">
            <p><i class="fa-solid fa-copyright"></i> Copyright 2012-2020 | Avada Theme by Theme Fusion | All Rights Reserved | Powered by WordPress</p>
        </div>
     </div>
</template>

<script>
export default {
    name: 'FooterContent',
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

img{
    display: block;
}
.btn-footer{
    color: $light_gold;
    padding: .8rem 2rem;
    background-color: transparent;
    border: 2px solid $light_gold;
    cursor: pointer;
    margin-top: 4rem;

    &:hover{
        color: $drift_wood;
        border: 2px solid $drift_wood;
    }
}

.container-footer{
    height: 60vh;
    background-color: $cod_gray ;
    .flex{
        display: flex;
        justify-content: center;
        text-align: center;
        gap: 3rem;
        padding-bottom: 3.5rem;

        .left, .right{
            padding-top: 4rem;
        }

        .center{
            padding-top: 3rem;

            img{
                padding-bottom: 3rem;
            }

            ul{
                padding-bottom: 3rem;
            }

            li{
                color: $emperor;
                padding: .2rem;
                list-style: none;
                a{
                    color: $emperor;
                    text-decoration: none;
                }
            }

            p{
                font-size: 15px;
                color: $light_gold;
            }

            .icons{
                padding-top: 1.5rem;
                li{
                    display: inline-block;
                    padding: 0 .7rem;
                    color: white;
                }
            }
        }
    }

    .foot{
        height: 10vh;
        background-color: $dark_gray;
        color: $mine_shaft;

        display: flex;
        justify-content: center;
        align-items: center;
    }
}
</style>