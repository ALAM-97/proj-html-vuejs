<template>
    <ul>
        <li v-for="(course, index) in courses" :key="index">
            <img :src="course.img" alt="">
            <div class="free" v-if="(course.free == true) ? 'free' : null">FREE</div>
            <div class="infos">
                <div class="price">${{course.price}}.<span>00</span></div>
                <div class="course-title">{{course.title}}</div>
                <div class="less-and-stud">
                    <div class="lessons">
                        <i class="far fa-file-alt"></i>
                        {{course.lessons}} Lessons
                    </div>
                    <div class="students">
                        <i class="far fa-user"></i>
                        {{course.students}} Students
                    </div>
                </div>
            </div>
        </li>
    </ul>
</template>

<script>
export default {
    name: 'CourseCard',
    data() {
        return {
            courses: [
                {
                    img : require("../assets/images/course-02-480x298.jpg"),
                    price : "40",
                    title : "Learning to Write as a Professional Author",
                    lessons : "20",
                    students : "50",
                    free: false
                },
                {
                    img : require("../assets/images/stock-full-hd-03-480x298.jpg"),
                    price : "0",
                    title : "Customer-Centric Info-Tech Strategies",
                    lessons : "24",
                    students : "769",
                    free: true
                },
                {
                    img : require("../assets/images/stock-full-hd-04-480x298.jpg"),
                    price : "19",
                    title : "Open Programming Courses for everyone: python",
                    lessons : "17",
                    students : "62",
                    free: false
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
        li {
            width: calc(100% / 3 - 1.25rem);
            display: flex;
            flex-direction: column;
            height: 25rem;
            border-radius: .3125rem;
            position: relative;
        }
        
        img {
            border-radius: .3125rem .3125rem 0 0;
            width: 100%;
            height: 50%;
        }
        .free {
                width: 70px;
                height: 30px;
                background-color: #ee7455;
                color: $white;
                text-align: center;
                line-height: 30px;
                position: absolute;
                top: 0;
                right: 0;
            }
        .infos {
            width: 100%;
            height: 50%;
            padding: 1.5625rem;
            background-color: $white;
            border-radius: 0 0 .3125rem .3125rem;
            .price {
                font-size: 1.3rem;
                font-weight: 600;
                color: $detailsColor;
                margin-bottom: 10px;
                span {
                    font-size: 1.1rem;
                }
            }
            .course-title {
                font-weight: 600;
                font-size: 1.2rem;
                margin-bottom: 30px;
            }
            .less-and-stud {
                display: flex;
                .lessons,
                .students {
                    font-size: .9rem;
                    font-weight: 300;
                    color: #9693aa;
                    margin-right: 20px;
                }
            }
        }
    }

</style>