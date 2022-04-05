<template>
    <div class="container-blog">
        <div class="triangle"></div>
        <div class="title">
            <p>TALES FORM THE BARBER SHOP</p>
            <h2>Recent Blog Posts</h2>
        </div>

        <div class="blog">
            <div class="item" v-for="element in arrBlogUser" :key="element.id">
                <div class="img-fix">
                    <img :src="element.img" :alt="element.title">
                </div>
                <h3>{{ element.title }}</h3>
                <p>{{ element.text }}</p>
            </div>
        </div>

        <button class="btn-blog">READ MORE FROM OUR BLOG</button>
    </div>
</template>

<script>
import blog1 from'../../public/img/avadabarbers-second-blog-320x202.jpg'
import blog2 from'../../public/img/avadabarbers-choosing-blog-320x202.jpg'
import blog3 from'../../public/img/avadabarbers-ourservice-blog-320x202.jpg'

export default {
    name: 'BlogContent',
    data () {
        return {
            arrBlogUser: 
            [
                {
                    id: 1,
                    img: blog1,
                    title: 'Avada Barber Now Open',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos asperiores nobis voluptates.',
                },
                {
                    id: 2,
                    img: blog2,
                    title: 'Choosing The Right Barber',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos asperiores nobis voluptates.',
                },
                {
                    id: 3,
                    img: blog3,
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
    height: 95vh;
    text-align: center;
    background-color: $light_silver;
    position: relative;
}

.triangle{
    width: 100%;
    height: 100px;
    background-color: white;
    clip-path: polygon(50% 100%, 0 0%, 100% 0%);
    position: absolute;
    top: 0;
    left: 0;
}

.title{
    width: 1000px;
    margin: 0 auto;
    text-align: center;
    padding-top: 10rem;
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

        .img-fix{
            width: 320px;
            height: 202px;
            overflow: hidden;
            cursor: pointer;
        }

        img:hover{
            transform: scale(1.1);
            opacity: .9;
            transition: 1s ease;
        }

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
        color: $bean;
        border: 2px solid $bean;
    }
}
</style>