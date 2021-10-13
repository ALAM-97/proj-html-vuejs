<template>
    <div class="hero">
        <div class="info">
            <h2>Commence Business</h2>
            <h1>Distant Mentoring Program</h1>
            <button class="btn">
                Download the guidebook 
                <i class="fas fa-long-arrow-alt-right"></i>
            </button>
        </div>
        
    </div>
</template>

<script>

export default {
    name: 'Hero'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';
    
    .hero {
        background-image: url('../assets/images/home-3-hero-bg.jpg');
        background-size: cover;
        .info {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: $white;
            padding: 15rem 0;
            h2 {
            font-size: 1.7rem;
            }
            h1 {
                margin: .625rem 0;
                font-size: 3rem;
                font-weight: 400;
            }
            button {
                color: $detailsColor;
                transition: all .1s;
                &:hover {
                    color: $white;
                    background-color: $detailsColor;
                }
            }
        }
        
    }

</style>