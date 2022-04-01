<template>
    <div class="container">
        <div class="title">
            <p>WHAT PEOPLE SAY</p>
            <h2>Review</h2>
        </div>

        <div class="item" >
            <div class="review" v-for="element in arrReviewUser" :key="element.id">
                <p class="txt-user">{{ element.text }}</p>
                <img src="../../public/img/avadabarbers-trimcut-gallery6-200x200.jpg" alt="">
                <p class="name-user">{{ element.userName }}</p>
            </div>        
        </div>
        <div class="triangle"></div>
    </div>
</template>

<script>
export default {
    name: 'ReviewContent',
    data () {
        return {
            arrReviewUser:
            [
                {
                    id: 1,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: '',
                    userName: 'John Doe',
                },
                {
                    id: 2,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: '',
                    userName: 'Pete Jones',
                },
                {
                    id: 3,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: '',
                    userName: 'Mark Wilson',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container{
    height: 70vh;
}
.title{
    width: 1000px;
    margin: 0 auto;
    margin-top: 1rem;
    text-align: center;

    p{
        color: $drift_wood;
        font-size: 15px;
    }
    h2{
        font-size: 50px;
        color: $silver;
        margin-bottom: 3rem;
    }
}

.item{
    width: 1000px;
    margin: 0 auto;
    display: flex;
    gap: 5rem;

    .review{
        width: calc(100% / 3 ); 
        text-align: center;
        img{
            border-radius: 50%;
            margin-bottom: 1rem;
        }
        
        .txt-user{
            font-size: 15px;
            line-height: 25px;
            color: $silver;
            margin-bottom: 1.5rem;
        }
        .name-user {
            color: $drift_wood;
            font-style: italic;
        }
    }
}

.triangle{
    width: 100%;
    height: 100px;
    background-color: #121315;
    clip-path: polygon(50% 100%, 0 0, 100% 0);
    position: absolute;
    top: 837px;
    left: 0;
}
</style>