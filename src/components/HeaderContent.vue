<template>
  <div class="container-header">
    
    <!-- NAV BAR LOGO + ICONS -->
    <nav>
        <img src="../../public/img/avadabarbers-stickylogo-x1.png" alt="logo barber-shop">
        <div class="icon">
            <i class="fa-solid fa-cart-shopping"></i>
            <i class="fa-solid fa-bars"></i>
        </div>
    </nav>


    <div class="main">
        <!-- section title -->
        <div class="title">
            <h1>Barber Shop</h1>
            <div class="line"></div>
            <p>The Pinnacle of Male Grooming</p>
            <button class="btn-nav">LEARN MORE</button>
        </div>

        <!-- img -->
        <div class="img-under-nav">
            <img src="../../public/img/avadabarbers_hero_focalmirror-400x550.png" alt="">
        </div>

    </div>
  </div>

</template>

<script>

export default {
    name: 'HeaderContent',
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container-header{
    width: 100%;
    height: 90vh;
    background-image: url(../../public/img/avadabarbers-homepage-hero-bg.jpg);
    background-size: cover
}

nav{
    width: 1000px;
    height: 100px;
    margin: 0 auto;

    display: flex;
    justify-content: space-between;
    align-items: center;

    .icon{
        color: white;
        .fa-cart-shopping{
            font-size: 15px;
            margin-right: 1rem;
        }

        .fa-bars{
            font-size: 20px;
        }
    }
}

.main{
    width: 1200px;
    margin: 0 auto;
    display: flex;
}

.title{
    width: 45%;
    height: calc(90vh - 300px);
    margin: 0 auto;
    margin-top: 180px;
    
    h1{
        color: white;
        font-size: 70px;
        font-family: 'Abril Fatface', cursive;
        padding-bottom: .8rem;
    }

    .line{
        width: 200px;
        height: 3px;
        background-color: $light_gold;
        margin-bottom: 1.7rem;
    }

    p{
        color: #505050 ;
        margin-bottom: 1.7rem;
    }

    .btn-nav{
        color: $light_gold;
        padding: .8rem 2rem;
        background-color: transparent;
        border: 2px solid $light_gold;
        cursor: pointer;
        &:hover{
            transform: scale(1.1);
        }
    }

}

.img-under-nav{
    width: 40%;
}
</style>