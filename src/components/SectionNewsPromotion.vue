<template>
    <section class="news-promotions section-C">
         <!-- Heading Section -->
        <div class="heading-section">
            <h2 class="title">Latest news & promotions</h2>
            <div class="line-separator"></div>
        </div>

        <div class="ms_secondary_container">
            <!-- Column -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <img src="../assets/img/blog92x-600x687.jpg" alt="">
                    <h3 class="title">Braised Abalone</h3>
                    <div class="meta-data">
                        By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a>
                    </div>
                </div>
            </div>
            <!-- Column -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <img src="../assets/img/blog72x-600x687.jpg" alt="">
                    <h3 class="title">Braised Abalone</h3>
                    <div class="meta-data">By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a></div>
                </div>
            </div>
            <!-- Column -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <img src="../assets/img/blog82x-600x687.jpg" alt="">
                    <h3 class="title">Braised Abalone</h3>
                    <div class="meta-data">By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a></div>
                </div>
            </div>
            
            
            
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionNewsPromotion'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.news-promotions.section-C {
    padding: 8rem 0;

    .ms_secondary_container {

        .ms_col {
            
            .ms_card {
                flex-direction: column;
                align-items: center;
                color: $ms_black;
                text-align: center;

                img {
                    max-width: 100%;
                    margin-bottom: 1rem;
                    height: 40rem;
                    object-fit: cover;
                }
                .title {
                    font-size: 2rem;
                    margin-bottom: 0;
                    font-weight: 400;
                }
                .meta-data {
                    font-family: 'Lora', Arial, Helvetica, sans-serif;
                    font-size: 0.8rem;

                    a {
                        font-weight: 600;

                        &:hover {
                            text-decoration: underline;
                        }
                    }
                }
            }
        }
    }
}
</style>