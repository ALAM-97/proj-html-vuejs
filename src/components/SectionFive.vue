<template>
    <div class="container">
            <section>
                <div class="left-section">
                    <div>TESTIMONIALS</div>
                    <h4>
                        Why Do People <span>*Hearts*</span> Us?
                    </h4>
                    <p>
                        Seeking for verbals of our service quality? Find them here. Everything in transparent and straightforward for your sense of justification.
                    </p>
                    <div class="link">
                        <a class="dark-link" href="#">View all 
                            <i class="fas fa-long-arrow-alt-right"></i>
                        </a>
                    </div>
                </div>
                <div class="right-section">
                    <div class="first-card">
                        <div class="card-title">
                            Professional team of spoecialists and passionate mentors at reach
                        </div>
                        <p>
                            I need to get a certification for English proficuency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.
                        </p>
                        <div class="user-info">
                            <img src="../assets/images/testimonial-avata-01.jpg" alt="">
                            <div class="user-name">
                                <div class="name">MADLEY PONDOR</div>
                                <div class="work">/ IT Specialist</div>
                            </div>
                        </div>
                    </div>
                    <div class="bg-card">
                        <div class="card-title">
                            The MaxCoach team works really hard to ensure high level of quality
                        </div>
                        <p>
                            I am happy with their arrangement of lessons and subjects. They are really the best online tutors I have ever found, I recommend them.
                        </p>
                        <div class="user-info">
                            <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                            <div class="user-name">
                                <div class="name">MINA HOLLACE</div>
                                <div class="work">/ Freelancer</div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>
</template>

<script>
export default {
name: 'SectionFive'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    section {
        display: flex;
        justify-content: space-between;
        position: relative;
        padding-top: 15rem;
        .left-section {
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 35%;
            div {
                font-size: .9rem;
                margin-left: .3125rem;
                span {
                    font-weight: 600;
                }
            }
            .link {
                font-size: 1rem;
            }
        }
        .right-section {
            width: 55%;
            position: relative;
            .first-card {
                width: 100%;
                padding: 2.5rem 2.8125rem;
                border-radius: .3125rem;
                box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.10);
                background-color: $white;
                z-index: 1;
            }
            .bg-card {
                width: 80%;
                height: 37.5rem;
                padding: 2.5rem 2.8125rem;
                border-radius: .3125rem;
                position: absolute;
                left: 50%;
                top: -43%;
                transform: translate(-50%);
                display: flex;
                flex-direction: column;
                box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.10);
                opacity: .5;
                z-index: -1;
                .user-info {
                    margin-top: auto;
                }
            }
            .card-title {
                    font-weight: 700;
                }
                p {
                    margin-top: 1.25rem;
                    margin-bottom: 2.8125rem;
                    font-size: .9rem;
                }
            .user-info {
                display: flex;
                align-items: center;
                img {
                    width: 14%;
                    border-radius: 50%;
                    margin-right: 1.25rem;
                }
                .name {
                    font-weight: 700;
                    margin-bottom: 10px;
                }
                .work {
                    font-weight: 300;
                    font-size: .9rem;
                }
            }
        }
    }


</style>