<template>
    <div class="footer-bg">
        <div class="container">
            <section>
                <div class="footer-top">
                    <div class="footer-left">
                        <h6>Address</h6>
                        <ul>
                            <li v-for="(info, index) in infos" :key="index">
                                {{info}}
                            </li>
                        </ul>
                        <ul class="socials">
                            <li><i class="fab fa-facebook-square"></i></li>
                            <li><i class="fab fa-twitter"></i></li>
                            <li><i class="fab fa-instagram"></i></li>
                            <li><i class="fab fa-linkedin"></i></li>
                        </ul>
                    </div>
                    <div class="footer-right">
                        <div class="left">
                            <h6>Explore</h6>
                            <ul>
                                <li v-for="(link, index) in explore" :key="index">
                                    {{link}}
                                </li>
                            </ul>                   
                        </div>
                        <div class="right">
                            <h6>Information</h6>
                            <ul>
                                <li v-for="(link, index) in information" :key="index">
                                    {{link}}
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="footer-bottom">
                    <i class="far fa-copyright"></i> 2020 Maxcoach. All Rights Reserved
                </div>
            </section>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            infos: [ "382 NE 191st St # 87394 Miami, FL 33179-3899", "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)", "support@maxcoach.com"],
            explore: ["Start here", "Blog", " About us", "Success story", "Courses", "Contact us"],
            information: ["Membership", "Purchase guide", "Privacy policy", "Terms of service"]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/common.scss";

    section {
        padding: 3.75rem 0 2.5rem 0;
        color: $white;
        display: flex;
        flex-direction: column;
        .footer-top {
            display: flex;
            justify-content: space-between;
        }
        h6 {
            font-size: 1rem;
            margin-bottom: .625rem;
        }
        li {
            color: #8b8b90;
            font-size: .9rem;
            margin-bottom: .625rem;
            &:hover {
                    color: $lightGray;
                }
        }
        .socials {
            display: flex;
            li {
                margin-top: .625rem;
                margin-right: 1.25rem;
                font-size: 1.7rem;
            }
        }
        .footer-left {
            width: 35%;
        }
        .footer-right {
            display: flex;
            width: 50%;
            .left {
                padding-left: 3.125rem;
                ul {
                    display: grid;
                    grid-template-rows: repeat(3, 2.1875rem);
                    grid-template-columns: repeat(2, 9.375rem);
                }
            }
            .right {
                margin-left: 1.25rem;
                ul {
                    display: grid;
                    grid-template-rows: repeat(4, 2.1875rem);
                }
            }
        }
    }
    .footer-bottom {
            color: #8b8b90;
            text-align: center;
            margin-top: 3.125rem;
            .fa-copyright {
                font-size: .7rem;
                vertical-align: middle;
            }
        }

</style>