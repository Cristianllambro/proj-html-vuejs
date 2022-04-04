<template>
    <div class="container-review">
        <div class="title">
            <p>WHAT PEOPLE SAY</p>
            <h2>Review</h2>
        </div>

        <div class="item" >
            <div class="review" v-for="element in arrReviewUser" :key="element.id">
                <p class="txt-user">{{ element.text }}</p>
                <img :src="element.img" :alt="element.userName">
                <p class="name-user">{{ element.userName }}</p>
            </div>        
        </div>
        <div class="triangle"></div>
    </div>
</template>

<script>
import user1 from '../../public/img/avadabarbers-trimcut-gallery6-200x200.jpg'
import user2 from '../../public/img/avadabarbers-trimcut-gallery7-200x201.jpg'
import user3 from '../../public/img/avadabarbers-trimcut-gallery3-200x201.jpg'
export default {
    name: 'ReviewContent',
    data () {
        return {
            arrReviewUser:
            [
                {
                    id: 1,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: user1,
                    userName: 'John Doe',
                },
                {
                    id: 2,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: user2,
                    userName: 'Pete Jones',
                },
                {
                    id: 3,
                    text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione dicta asperiores, ipsum aut deserunt, perferendis vitae exercitationem atque ut possimus dolores ab at qui quas consequatur nemo aliquam doloremque ipsam!',
                    img: user3,
                    userName: 'Mark Wilson',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";

.container-review{
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

</style>