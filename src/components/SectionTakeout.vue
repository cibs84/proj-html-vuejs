<template>
    <!-- SECTION-A - Takeout Now Available -->
    <section class="takeout section-A">
        
        <!-- Col Image -->
        <div class="ms_col image">
            <img src="../assets/img/slider72x-scaled.jpg" alt="">
            <div class="overlay"></div>
        </div>

        <!-- Col Text -->
        <div class="ms_col text">
            <!-- Card-a -->
            <div class="card-a">
                <!-- Line Separator -->
                <div class="line-separator"></div>
                <!-- Content -->
                <div class="content">
                    <div class="above-title">Enjoy your meal at home</div>
                    <h2 class="title">Takeout now available</h2>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <!-- Button -->
                    <a href="#">
                        <span class="car-icon"><i class="fa-solid fa-car"></i></span>
                        View takeout menu
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionTakeout'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';
.takeout {

    .ms_col.image {

        img {
            object-position: bottom;
        }
    }
    .car-icon {
        margin-right: 0.5rem;
        font-size: 0.9rem;
    }
}
</style>