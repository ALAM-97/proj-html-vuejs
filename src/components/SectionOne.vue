<template>
    <div class="gray-bg">
        <div class="container">
            <section>
                <!-- details image -->
                <img class="detail-one" src="../assets/images/maxcoach-shape-07.png" alt="">
                <img class="detail-two" src="../assets/images/maxcoach-shape-02.png" alt="">
                <div class="brown-circle"></div>
                <div class="left-section">
                    <div>EVERYTHING IN <span>MAXCOACH</span></div>
                    <h4>
                        Learn about our <span>Work Culture</span> at MaxCoach
                    </h4>
                    <p>
                        Spend some time to visit our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classe every beginning of each month.
                    </p>
                    <div class="link">
                        Have questions? 
                        <a href="#">Get Free Guide 
                            <i class="fas fa-long-arrow-alt-right"></i>
                        </a>
                    </div>
                </div>
                <div class="right-section">
                    <img src="../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
                    <img class="absolute-img" src="../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
                </div>
            </section>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionOne'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    section {
        display: flex;
        justify-content: space-between;
        padding-top: 12.5rem;
        position: relative;
        .detail-one {
            position: absolute;
            width: 10%;
            top: 27%;
            right: 9%;
            z-index: 0;
        }
        .detail-two {
            position: absolute;
            width: 10%;
            bottom: -14%;
            right: 9%;
            z-index: 2;
        }
        .brown-circle {
            left: 40%;
            top: 32%;
        }
        .left-section {
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 40%;
            div {
                font-size: .9rem;
                margin-left: .3125rem;
                span {
                    font-weight: 600;
                }
            }
            .link {
                font-size: 1rem;
                a {
                    color: $detailsColor;
                    font-weight: bold;
                }
            }
        }
        .right-section {
            position: relative;
            width: 50%;
            img {
                width: 90%;
                height: 100%;
                border-radius: .3125rem;
            }
            .absolute-img {
                position: absolute;
                width: 35%;
                height: 47%;
                top: -20%;
                right: -5%;
            }
        }
    }

</style>