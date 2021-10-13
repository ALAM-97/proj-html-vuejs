<template>
    <div class="container">
        <section>
            <!-- details image -->
            <img class="detail-one" src="../assets/images/maxcoach-shape-02.png">
            <img class="detail-two" src="../assets/images/maxcoach-shape-09.png">
            <div class="lightgreen-circle"></div>
            <div class="section-title">
                <h4>Subscribe <span>Newsletter</span></h4>
                <div>Enter your email address to register to our newsletter subscription <br> delivered on a regulkar basis!</div>
            </div>
            <div class="email-input">
                <input type="email" placeholder="Enter your email">
                <button>
                    Subscribe
                </button>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: "SectionEight"
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
    section {
        margin-bottom: 100px;
        position: relative;
        .detail-one {
            position: absolute;
            right: -7%;
            top: 50%;
        }
        .detail-two {
            position: absolute;
            right: -12%;
            top: 20%;
        }
        .lightgreen-circle {
            position: absolute;
            left: 0;
            top: 65%;
            opacity: .7;
        }
    }
    .section-title {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 3.125rem 0 3.125rem 0;
        margin: 0 auto;
        div {
            margin-left: .3125rem;
            text-align: center;
            color: $mediumGray;
        }
    }
    .email-input {
        text-align: center;
        input {
            width: 42%;
            height: 50px;
            border-radius: 5px 0 0 5px;
            border: none;
            background-color: $lightGray;
            padding: 0 15px;
            &:focus {
                outline-width: 0;
            }
        }
        button {
            height: 50px;
            width: 10%;
            border-radius: 0 5px 5px 0;
            border: none;
            background-color: $detailsColor;
            color: $white;
            font-weight: 600;
            transition: all .1s;
            &:hover {
                background-color: $white;
                color: $detailsColor;
                border: .125rem solid $detailsColor;
            }
        }
    }

</style>