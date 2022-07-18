<template>
    <section class="features section-C">
        <div class="ms_secondary_container">
            <!-- Column -->
            <div class="ms_col">
                <!-- Card-b -->
                <div class="card-b">
                    <img src="../assets/img/sushi-1.png" alt="shushi illustration">
                    <h3 class="title">Braised Abalone</h3>
                    <div class="line-separator"></div>
                    <p>Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.</p>
                    <!-- Button -->
                    <a href="#">Explore the menu</a>
                </div>
            </div>
            
            <!-- Column -->
            <div class="ms_col">
                <!-- Card-b -->
                <div class="card-b">
                    <img src="../assets/img/sushi-2.png" alt="shushi illustration">
                    <h3 class="title">Perfect for groups</h3>
                    <div class="line-separator"></div>
                    <p>Hendrerit amet, volutpat leo non, commodo maecenas scelerisque tincidunt. Morbi vulputate morbi purus quisque sit sagittis orci elementum gravida.</p>
                    <!-- Button -->
                    <a href="#">Make a reservation</a>
                </div>
            </div>
            
            <!-- Column -->
            <div class="ms_col">
                <!-- Card-b -->
                <div class="card-b">
                    <img src="../assets/img/sushi-3.png" alt="shushi illustration">
                    <h3 class="title">Fresh produce everyday</h3>
                    <div class="line-separator"></div>
                    <p>Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.</p>
                    <!-- Button -->
                    <a href="#">Learn more about us</a>
                </div>
            </div>
            
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionFeatures'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.features.section-C {
    padding-bottom: 8rem;

    .ms_secondary_container {

        .ms_col {
            
            .card-b {
                flex-direction: column;
                align-items: center;
                color: $ms_black;
                text-align: center;
                padding: 0 1.5rem;

                img {
                    width: 6rem;
                    margin-bottom: 1rem;
                }
                .title {
                    font-size: 2rem;
                    margin-bottom: 0;
                }
                .line-separator {
                    margin-right: 0;
                    margin-bottom: 1.5rem;
                }
                a {
                    border-color: $ms_silver;

                    &:hover {
                        color: white;
                        background-color: $ms_black;
                    }
                }
                p {
                    font-size: 1.1rem;
                }
            }
        }
    }
}
</style>