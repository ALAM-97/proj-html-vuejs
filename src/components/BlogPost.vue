<template>
    <ul>
        <li v-for="(post, index) in posts" :key="index">
            <img :src="post.img" alt="">
            <div class="profession">{{post.profession}}</div>
            <div class="post-title">{{post.title}}</div>
            <div class="info">
                <div class="date">
                    <i class="far fa-calendar"></i>
                    {{post.date}}
                </div>
                <div class="views">
                    <i class="far fa-eye"></i>
                    {{post.views}}
                </div>
            </div>
            
        </li>
    </ul>
</template>

<script>
export default {
    name: 'BlogPost',
    data() {
        return {
            posts: [
                {
                    img: require("../assets/images/artist-blog-03-480x325.jpeg"),
                    profession: "ARTIST",
                    title: "Brush Strokes Energize Trees in Paintings",
                    date: "May 15, 2020",
                    views: "688 views"
                },
                {
                    img: require("../assets/images/artist-blog-01-480x325.jpg"),
                    profession: "ARTIST",
                    title: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    date: "Oct 19, 2020",
                    views: "603 views"
                },
                {
                    img: require("../assets/images/artist-blog-02-480x325.jpg"),
                    profession: "ARTIST",
                    title: "Connection Between Self-Portraits and Identity",
                    date: "Nov 11, 2020",
                    views: "397 views"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

    ul {
        display: flex;
        justify-content: space-between;
        width: 100%;
        li {
            width: calc(100% / 3 - 1.25rem);
            img {
                width: 100%;
                border-radius: .3125rem;
            }
            .profession {
                font-weight: 300;
                font-size: .9rem;
                margin: .625rem 0;
            }
            .post-title {
                font-size: 1.1rem;
                font-weight: 600;
                line-height: 1.875rem;
                margin-bottom: 20px;
            }
            .info {
                display: flex;
                .date,
                .views {
                    font-size: .9rem;
                    font-weight: 300;
                    color: #9693aa;
                    margin-right: 20px;
                }
            }
        }
    }

</style>