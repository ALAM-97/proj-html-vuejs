<template>
    <div class="gray-bg">
        <div class="container">
            <section>
                <!-- details image -->
                <img class="detail-one" src="../assets/images/maxcoach-shape-07.png" alt="">
                <img class="detail-two" src="../assets/images/maxcoach-shape-05.png" alt="">
                <img class="detail-three" src="../assets/svg/svg-0.svg" alt="">
                <div class="brown-circle"></div>
                <div class="left-section">
                    <div class="video"></div>
                    <img class="absolute-img" src="../assets/images/icon-youtube-play.png" alt="">
                </div>
                <div class="right-section">
                    <div>HOW WE WORK</div>
                    <h4>
                        Upgrade Your Skills <span>Upgrade Your Life</span>
                    </h4>
                    <p>
                        Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets on insights into your career. MaxCoach accompany leanerners in every stage of learning.
                    </p>
                    <div class="link">
                        <a class="dark-link" href="#">Download free guidebook 
                            <i class="fas fa-long-arrow-alt-right"></i>
                        </a>
                    </div>
                </div>
            </section>
        </div>
    </div>
    
</template>

<script>
export default {
    name: 'SectionThree'
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    .detail-one {
        position: absolute;
        bottom: -20%;
        left: 35%;
    }
    .detail-two {
        position: absolute;
        left: -10%;
        top: 8%;
    }
    .detail-three {
        position: absolute;
        top: -23%;
        left: -5%;
        opacity: .1;
    }
    .brown-circle {
        top: -8%;
        left: 58%;
    }
    .left-section {
        position: relative;
        width: 50%;
        height: 400px;
        overflow: hidden;
        border-radius: .3125rem;
        cursor: pointer;
        .video {
            background-image: url("../assets/images/stock-full-hd-11-670x450.jpg");
            background-size: cover;
            height: 100%;
            width: 100%;
            transition: all .6s;
        }
        .absolute-img {
                position: absolute;
                width: 15%;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
        &:hover .video,
        &:focus .video {
                transform: scale(1.1);
            }
    }
    .right-section {
        width: 40%;
        div {
            font-size: .9rem;
            margin-left: .3125rem;
        }
        .link {
            font-size: 1rem;
        }
    }
}
    

</style>