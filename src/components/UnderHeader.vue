<template>
    <div class="container">
        <div class="title">
            <p>AWARD WINNING</p>
            <h2>Pro Barbers</h2>
            <button class="btn-under">MEET YOUR NEW BARBER</button>
            <div class="triangle"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'UnderHeader',
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container{
    .title{
        height: 500px;
        text-align: center;
        padding-top: 6rem ;
        position: relative;

        background-image: url(../../public/img/avadabarbers-about-introbackground.jpg);
        background-size: cover;
       p{
           font-size: 14px;
           color: $light_gold;
        }
       h2{
           color: $silver;
           font-size: 50px;
           font-family: 'Abril Fatface', cursive;
           margin-bottom: 1.5rem;
       }
       .btn-under{
        color: $light_gold;
        padding: .8rem 2rem;
        background-color: transparent;
        border: 2px solid $light_gold;
        cursor: pointer;
        &:hover{
            color: $drift_wood;
            border: 2px solid $drift_wood;
        }
       }
    }
    .triangle{
        width: 100%;
        height: 100px;
        background-color: white;
        clip-path: polygon(50% 0%, 0 100%, 100% 100%);
        position: absolute;
        top: 400px;
        left: 0;
    }

}

</style>