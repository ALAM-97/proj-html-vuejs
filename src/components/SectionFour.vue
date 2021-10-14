<template>
    <div class="divider">
        <div class="gray-bg">
            <div class="container">
                <section>
                    <div class="section-title">
                        <div>JOIN MAXCOACH AT BEST</div>
                        <h4>Latest Online <span>Courses</span></h4>
                    </div>
                    <div class="services">
                        <CourseCard/>
                    </div>
                    <div class="courses-nav">
                        <i class="fas fa-circle active"></i>
                        <i class="fas fa-circle"></i>
                        <i class="fas fa-circle"></i>
                        <i class="fas fa-circle"></i>
                        <i class="fas fa-circle"></i>
                    </div>
                    <div class="courses-sub">
                        Control your personal preference settings to get notified about <br> appropiate courses.
                        <a class="dark-link" href="#">View all courses <i class="fas fa-long-arrow-alt-right"></i></a>
                    </div>
                </section>
            </div>
        </div>
        <Divider class="abs"/>
    </div>
    
</template>

<script>
import CourseCard from "./CourseCard.vue";
import Divider from "./Divider.vue"

export default {
    name: 'SectionFour',
    components: {
        CourseCard,
        Divider
    },
    
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

    .divider {
        position: relative;
        .abs {
            position: absolute;
            bottom: -0.625rem;
        }
    }
    .section-title {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 10.625rem 0 3.125rem 0;
        margin: 0 auto;
        div {
                font-size: .9rem;
                margin-left: .3125rem;
            }
    }
    .services {
        display: flex;
        justify-content: space-between;
    }
    .courses-nav {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 2.5rem auto;
        i {
            margin: 0 .625rem;
            opacity: .3;
            font-size: .6rem;
            &.active {
                opacity: .8;
                font-size: .9rem
            }
        }
    }
    .courses-sub {
        width: 100%;
        text-align: center;
        line-height: 2.1875rem;
        padding-bottom: 5rem;
    }

</style>