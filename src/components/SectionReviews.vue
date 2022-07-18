<template>
    <!-- SECTION-B - Reviews -->
    <section class="reviews section-B">
        <!-- Heading Section -->
        <div class="heading-section">
            <h2 class="title">What critics are saying about us</h2>
            <div class="line-separator"></div>
        </div>

        <!-- Container -->
        <div class="ms_secondary_container">

             <!-- Col Image -->
            <div class="ms_col main image">
                <img src="../assets/img/blog72x-800x916.jpg" alt="">
            </div>

            <!-- Col Text -->
            <div class="ms_col main text">
                <!-- Card-b -->
                <div class="card-b">
                    <!-- Heading -->
                    <div class="above-title">Meggie Stewart</div>
                    <h3 class="title">New York Times</h3>
                    <!-- Stars -->
                    <div class="stars">
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                    </div>
                    <!-- Line Separator -->
                    <div class="line-separator"></div>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <p>Mauris in ligula sapien. Donec suscipit lectus.</p>
                    <!-- Button -->
                    <a href="#">Read full article</a>
                </div>
            </div>

            <!-- Col Text-Image -->
            <div class="ms_col text bg-img">
                <div class="ms_overlay"></div>
                <!-- Card-b -->
                <div class="card-b">
                    <!-- Heading -->
                    <div class="above-title">Mary Maxey</div>
                    <h3 class="title">The Guardian</h3>
                    <!-- Stars -->
                    <div class="stars">
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                    </div>
                    <!-- Line Separator -->
                    <div class="line-separator"></div>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <p>Mauris in ligula sapien. Donec suscipit lectus.</p>
                    <!-- Button -->
                    <a href="#">Read full article</a>
                </div>
            </div>

            <!-- Col Text-Image -->
            <div class="ms_col text bg-img">
                <div class="ms_overlay"></div>
                <!-- Card-b -->
                <div class="card-b">
                    <!-- Heading -->
                    <div class="above-title">Patrick Monroe</div>
                    <h3 class="title">Globe and Mail</h3>
                    <!-- Stars -->
                    <div class="stars">
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                        <span><i class="fa-solid fa-star"></i></span>
                    </div>
                    <!-- Line Separator -->
                    <div class="line-separator"></div>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <p>Mauris in ligula sapien. Donec suscipit lectus.</p>
                    <!-- Button -->
                    <a href="#">Read full article</a>
                </div>
            </div>

        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionReviews'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.section-B.reviews {
        padding: 8rem 0;
    
    .ms_secondary_container {
        row-gap: 3rem;

        .ms_col {
            max-width: 50%;
            width: calc(50% - 1.5rem);
        }
        .ms_col.bg-img {
            background-size: cover;
            position: relative;
            height: 44rem;
        }
        > :nth-child(3) {
            background-image: url('../assets/img/info52x.jpg');
        }
        > :nth-child(4) {
            background-image: url('../assets/img/info12x.jpg');
        }
        .ms_col.main {
            width: 50%;
        }
        .ms_col.text {
            padding: 0 10%;
            
            .card-b {
                flex-direction: column;
                align-items: flex-start;

            }
        }
    }
}
</style>