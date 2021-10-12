<template>
    <div class="gray-bg">
        <div class="container">
            <section>
                <div class="section-title">
                    <div>READ FOR MORE JOYMENT</div>
                    <h4>Latest From <span>Our Blogs</span></h4>
                </div>
                <div class="services">
                    <BlogPost/>
                </div>
            </section>
        </div>
    </div>
</template>

<script>
import BlogPost from './BlogPost.vue'

export default {
    name: 'SectionSeven',
    components: {
        BlogPost
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

    section {
        padding-bottom: 6.25rem;
    }
    .section-title {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 6.25rem 0 3.125rem 0;
        margin: 0 auto;
        div {
            font-size: .9rem;
            margin-left: .3125rem;
        }
        h4 {
            font-size: 2.9rem;
            margin: 1.25rem 0;
            font-weight: 600;
            line-height: 3.2rem;
            span {
                color: $detailsColor;
                font-weight: 300;
            }
        }
    }
    .services {
        display: flex;
        justify-content: space-between;
        
    }
</style>