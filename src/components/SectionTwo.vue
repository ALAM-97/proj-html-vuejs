<template>
    <div class="gray-bg">
        <div class="container">
            <section>
                <div class="numbers">
                    <div class="info-one">
                        129+ 
                        <span>ENROLLED LEARNERS</span>
                    </div>
                    <div class="info-two">
                        80
                        <span>FINISHED SESSIONS</span>
                    </div>
                    <div class="info-three">
                        4%
                        <span>SATISFACTION RATE</span>
                    </div>
                </div>
            </section>
        </div>
    </div>
        
</template>

<script>
export default {
    name: 'SectionTwo'
}
</script>

<style lang="scss">
@import "../assets/style/common.scss";

    section {
        width: 100%;
        .numbers {
            display: flex;
            width: 70%;
            justify-content: space-around;
            padding-top: 7.5rem;
            padding-bottom: 7.5rem;
            margin: 0 auto;
        }
        .info-one,
        .info-two,
        .info-three {
            display: flex;
            flex-direction: column;
            align-items: center;
            font-size: 2.5rem;
            font-weight: 700;
            color: $detailsColor;
            span {
                font-size: 1rem;
                font-weight: 600;
                color: $mediumGray;
            }
        }
    }

</style>