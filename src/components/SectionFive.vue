<template>
    <div></div>
</template>

<script>
export default {
name: 'SectionFive'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    section {
        background-color: #fff;
        display: flex;
        justify-content: space-between;
        color: $darkGray;
        position: relative;
        .detail-one {
            position: absolute;
            width: 10%;
            top: -17%;
            right: 11%;
            z-index: -1;
        }
        .detail-two {
            position: absolute;
            width: 10%;
            bottom: -18%;
            right: 11%;
            z-index: 1;
        }
        .brown-circle {
            left: 40%;
            top: -7%;
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
            p {
                font-size: .8rem;
                margin-left: .3125rem;
                margin-bottom: 1.25rem;
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
                border-radius: 5px;
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