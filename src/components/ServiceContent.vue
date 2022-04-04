<template>
    <div class="container-service">

        <div class="title">
            <p>MENS GROOMING</p>
            <h2>Services</h2>
        </div>

        <!-- three object barber -->
        <div class="tools">

            <div class="cont-1" v-for="element in arrImgTools" :key='element.id'>
                <img :src="element.img" :alt="element.title">
                <h3>{{ element.title }}</h3>
                <p>{{ element.under_title }}</p>
            </div>

        </div>
        <button class="btn-main">READ ABOUT OUR SERVICES</button>
        <div class="triangle"></div>
    </div>
</template>

<script>
import trim from '../../public/img/avadabarbers-trimcut-icon-before.png'
import wash from '../../public/img/avadabarbers-washndry-icon.png'
import beard from '../../public/img/avadabarbers-beardtrim-icon.png'
export default {
    name: 'ServiceContent',
    data () {
        return {
            arrImgTools: 
            [
                {
                    id: 1,
                    img: trim,
                    title: 'Trims & Cut',
                    under_title: 'Avada Barbers are experts in the lickety split trim and hair cut. Quick but careful and ridiculously good looking.'
                },
    
                {
                    id: 2,
                    img: wash,
                    title: 'Wash & Dry',
                    under_title: 'Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurous fashion.'
                },

                {
                    id: 3,
                    img: beard,
                    title: 'Beard Tidy',
                    under_title: 'Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers.',
                }

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container-service{
    height: 100vh;
    text-align: center;
    position: relative;
}

img{
    height: 130px;
}

.title{
    text-align: center;
    padding: 5rem 0;
    

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

.tools{
    width: 1000px;
    margin: 0 auto;

    display: flex;
    gap: 5rem;
    

    img{
        width: 70px;
        padding-bottom: 1.5rem;
    }

    h3{
        color: $teak;
        font-size: 28px;
        font-family: 'Abril Fatface', cursive;
        padding-bottom: 2rem;
    }
    
    p{
        font-size: 15px;
        line-height: 25px;
        color: $silver;
    }

    .cont-1{
        width: calc(100% / 3);
        text-align: center;
    }
}

.btn-main{
    color: $teak;
    padding: .8rem 2rem;
    margin-top: 4rem ;

    background-color: transparent;
    border: 2px solid $teak;
    cursor: pointer;

    &:hover{
        transform: scale(1.1);
    }
}

    .triangle{
        width: 100%;
        height: 100px;
        background-color: #121315;
        clip-path: polygon(50% 0%, 0 100%, 100% 100%);
        position: absolute;
        top: 837px;
        left: 0;
    }

</style>