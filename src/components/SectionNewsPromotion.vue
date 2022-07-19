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
                    <div class="text-area">
                        <h3 class="title">Braised Abalone</h3>
                        <div class="meta-data">
                            By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a>
                        </div>
                    </div>

                    <!-- Card Hover Items -->
                    <div class="ms_overlay">
                        <span class="link-icon"><i class="fa-solid fa-link"></i></span>
                        <h3 class="title">The best coffee in town</h3>
                        <div class="meta-data">News</div>
                    </div>
                    <div class="hiding-element"></div>
                </div>
            </div>
            <!-- Column -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <img src="../assets/img/blog72x-600x687.jpg" alt="">
                    <div class="text-area">
                        <h3 class="title">Braised Abalone</h3>
                        <div class="meta-data">
                            By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a>
                        </div>
                    </div>
                    
                    <!-- Card Hover Items -->
                    <div class="ms_overlay">
                        <span class="link-icon"><i class="fa-solid fa-link"></i></span>
                        <h3 class="title">The best coffee in town</h3>
                        <div class="meta-data">News</div>
                    </div>
                    <div class="hiding-element"></div>
                </div>
            </div>
            <!-- Column -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <img src="../assets/img/blog82x-600x687.jpg" alt="">
                    <div class="text-area">
                        <h3 class="title">Braised Abalone</h3>
                        <div class="meta-data">
                            By <a href="#">admin</a> | January 7th, 2020 | Categories: <a href="#">News</a>
                        </div>
                    </div>
                
                    <!-- Card Hover Items -->
                    <div class="ms_overlay">
                        <span class="link-icon"><i class="fa-solid fa-link"></i></span>
                        <h3 class="title">The best coffee in town</h3>
                        <div class="meta-data">News</div>
                    </div>
                    <div class="hiding-element"></div>
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
    height: 70rem;

    .ms_secondary_container {

        .ms_col {
            
            .ms_card {
                flex-direction: column;
                align-items: center;
                color: $ms_black;
                text-align: center;
                position: relative;
                height: 45rem;
                cursor: pointer;

                img {
                    height: 100%;
                    object-fit: cover;
                    transition: all 0.2s;
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
                .text-area {
                        position: absolute;
                        top: calc(100% - 6rem);
                        bottom: 0;
                        left: 0;
                        right: 0;
                        background-color: #fff;
                        transition: all 0.2s;
                        z-index: 10;
                        padding: 2rem 0;
                }
                .ms_overlay {
                    background: linear-gradient(#000, #0000);
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: center;
                    z-index: 30;
                    color: white;
                    opacity: 0;
                    transition: all 0.2s;

                    .link-icon {
                        font-size: 1.3rem;
                        margin-bottom: 0.2rem;
                    }
                }
                .hiding-element {
                        top: calc(100% - 0rem);
                        position: absolute;
                        top: 100%;
                        bottom: 0;
                        left: 0;
                        right: 0;
                        background-color: #fff;
                        transition: all 0.2s;
                        z-index: 20;
                }
                &:hover {

                    .text-area {
                        top: 100%;
                    }
                    .ms_overlay {
                        opacity: 1;
                    }
                    .hiding-element {
                        bottom: -6rem;
                    }
                }
            }
        }
    }
}
</style>