<template>
  <div class="container">
    
    <!-- NAV BAR LOGO + ICONS -->
    <nav>
        <img src="../../public/img/avadabarbers-stickylogo-x1.png" alt="logo barber-shop">
        <div class="icon">
            <i class="fa-solid fa-cart-shopping"></i>
            <i class="fa-solid fa-bars"></i>
        </div>
    </nav>

    <!-- squares white -->
    <div class="squares">
        <div class="square1">1</div>
        <div class="square2">2</div>
    </div>

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
            <img src="" alt="">
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


.container{
    width: 100vw;
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

.squares{
    width: 100%;
    height: 200px;
}

.title{
    width: 1000px;
    height: calc(90vh - 100px);
    margin: 0 auto;
    
    h1{
        color: white;
        font-size: 50px;
        font-family: 'Abril Fatface', cursive;
        padding-bottom: .8rem;
    }

    .line{
        width: 150px;
        height: 3px;
        background-color: orange;
        margin-bottom: 1.2rem;
    }

    p{
        color: #505050 ;
        margin-bottom: 1.2rem;
    }

    .btn-nav{
        background-color: transparent;
        border: 2px solid ;
    }
}
</style>