<template>
    <div class="container">
            <section>
                <!-- details image -->
                <div class="detail-one"><img src="../assets/images/maxcoach-shape-07.png" alt=""></div>
                <div class="detail-two"><img src="../assets/images/maxcoach-shape-05.png" alt=""></div>
                <svg class="detail-three" xmlns="http://www.w3.org/2000/svg" width="200" height="202"><path class="elementor-shape-fill" d="M139.374 198.088c16.328 8.906 51.35-1.087 58.304-39.038 7.15-39.022-13.182-40.052-9.633-54.248 14.243-21.15 16.782-48.14 2.028-64.387-36.503-38.024-45.629 7.604-76.048-20.28C101.727 7.837 83.1-6.735 56.23 3.405 18.239 17.74 27.33 47.659 27.33 69.313c0 7.624-24.216 21.957-26.87 41.573-3.346 24.734 12.168 57.29 26.87 68.443 23.322 26.363 59.318 20.28 75.541 11.154 13.931-7.836 25.35 1.52 36.503 7.605z" style="fill: #20ad96" /></svg>
                <div class="detail-four"><img src="../assets/images/maxcoach-shape-01.png" alt=""></div>
                <div class="brown-circle"></div>
                <div class="left-section">
                    <img src="../assets/images/home-3-team-image.png" alt="">
                </div>
                <div class="right-section">
                    <div>EVERYTHING IN <span>MAXCOACH</span></div>
                    <h4>
                        We're Here To <span>Transform</span> You!
                    </h4>
                    <p>
                        As learners, people can enjoy great companionshio from MaxCoach mentors and educators. We can help you develpo and grow at you best.
                    </p>
                    <button class="btn">
                        Get Free Guide
                    </button>
                </div>
            </section>
        </div>
</template>

<script>
export default {
    name: 'SectionSix'
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

section {
    display: flex;
    justify-content: space-between;
    padding: 15.625rem 0 9.375rem 0;
    align-items: center;
    position: relative;
    .detail-one {
        position: absolute;
        bottom: 5%;
        left: 20.5%;
        z-index: -1;
    }
    .detail-two {
        position: absolute;
        left: -13%;
        top: 50%;
        transform: translateY(-50%);
    }
    .detail-three {
        position: absolute;
        top: 30%;
        left: -5%;
        z-index: -1;
        opacity: .5;
    }
    .detail-four {
        position: absolute;
        bottom: 22%;
        left: -20%;
    }
    .brown-circle {
        top: 25%;
        left: 57%;
    }
    .right-section {
        width: 40%;
        div {
            font-size: .9rem;
            margin-left: .3125rem;
            span {
                font-weight: 600;
            }
        }
        button {
            background-color: $detailsColor;
            color: $white;
            border: .125rem solid transparent;
            transition: all .1s;
            &:hover {
                background-color: $white;
                color: $detailsColor;
                border: .125rem solid $detailsColor;
            }
        }
    }
}

</style>