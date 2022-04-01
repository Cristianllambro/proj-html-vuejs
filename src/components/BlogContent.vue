<template>
    <div class="container-blog">
        <div class="title">
            <p>TALES FORM THE BARBER SHOP</p>
            <h2>Recent Blog Posts</h2>
        </div>

        <div class="blog">
            <div class="item" v-for="element in arrBlogUser" :key="element.id">
                <img src="../../public/img/avadabarbers-second-blog-320x202.jpg" alt="barber">
                <h3>{{ element.title }}</h3>
                <p>{{ element.text }}</p>
            </div>
        </div>

        <button class="btn-blog">READ MORE FROM OUR BLOG</button>
    </div>
</template>

<script>
export default {
    name: 'BlogContent',
    data () {
        return {
            arrBlogUser: 
            [
                {
                    id: 1,
                    img: '',
                    title: 'Avada Barber Now Open',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos asperiores nobis voluptates.',
                },
                {
                    id: 2,
                    img: '',
                    title: 'Choosing The Right Barber',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos asperiores nobis voluptates.',
                },
                {
                    id: 3,
                    img: '',
                    title: 'Quick Service Guide',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos asperiores nobis voluptates.',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/variable.scss";
.container-blog {
    height: 75vh;
    text-align: center;
}

.title{
    width: 1000px;
    margin: 0 auto;
    text-align: center;
    p{
        color: $teak;
        font-size: 15px;
    }
    h2{
        font-size: 50px;
        color: $silver;
        margin-bottom: 3rem;
    }
}

.blog{
    display: flex;
    justify-content: center;
    gap: 3rem;

    .item{
        width: 300px;
        text-align: center;

        h3{
            font-size: 30px;
            color: $drift_wood;
            margin-bottom: 1rem;
            margin-top: .8rem;
        }

        p{
            color: $silver;
            font-size: 15px;
            line-height: 25px;
        }

    }

}
.btn-blog{
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
</style>