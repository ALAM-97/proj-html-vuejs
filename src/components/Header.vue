<template>
    <header>
        <nav>
            <ul>
                <li v-for="(elm, index) in headerNav" :key="index">
                    {{elm}} <i class="fas fa-angle-down"></i>
                </li>
            </ul>
            
        </nav>
        <img src="../assets/images/dark-logo.png" alt="">
        <div class="shop-nav">
            <div class="shop-cart">
                <i class="fas fa-shopping-cart"></i>
                <div class="items-in-cart">0</div>
            </div>
            <i class="far fa-user"></i>
            <div class="input-search">
                <input type="text" placeholder="Search...">
                <i class="fas fa-search"></i>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return {
            headerNav: ["Home", "Pages", "Courses", "Features", "Blog", "Shop"]
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    header {
        display: flex;
        align-items: center;
        padding: 1.25rem 4.375rem;
        width: 100%;
        nav {
            color: $darkBlue;
            display: flex;
            ul {
                display: flex;
                li {
                    margin-right: 25px;
                    .fa-angle-down {
                        font-size: 11px;
                    }
                }
            }
        }
        img {
            text-align: center;
            margin: auto;
        }
        .shop-nav {
            display: flex;
            justify-content: right;
            align-items: center;
            color: $darkGray;
            width: calc(100% / 3);
            .shop-cart {
                position: relative;
                .items-in-cart {
                    position: absolute;
                    top: -0.625rem;
                    right: -0.5rem;
                    width: .9375rem;
                    height: .9375rem;
                    line-height: .9375rem;
                    text-align: center;
                    background-color: $lightGreen;
                    border-radius: 50%;
                    font-size: .625rem;
                    font-weight: 800;
                    color: $white;
                }
            }
            .fa-user {
                    margin: 0 1.5625rem;
            }
            .input-search {
                position: relative;
                input {
                background-color: #f5f5f5;
                height: 40px;
                padding: 0 .9375rem;
                border: none;
                border-radius: .3125rem;
                }
                .fa-search {
                    position: absolute;
                    right: .625rem;
                    top: 50%;
                    transform: translateY(-50%);
                    color: $lightGreen;
                }
            }
        }
    }
</style>