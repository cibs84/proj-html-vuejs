<template>
    <!-- SECTION-A - Jumbotron -->
    <section class="ms_jumbotron section-A">
        
        <!-- Col Image -->
        <div class="ms_col image">
            <img src="../assets/img/slider52x.jpg" alt="">
            <div class="ms_overlay"></div>
        </div>

        <!-- Col Text -->
        <div class="ms_col text">
            <!-- Card-a -->
            <div class="card-a">
                <!-- Line Separator -->
                <div class="line-separator"></div>
                <!-- Content -->
                <div class="content">
                    <div class="above-title">The best table in town</div>
                    <h1 class="title">Fine dining experience</h1>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <!-- Button -->
                    <a href="#">Explore the menu</a>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionJumbotron'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

// Section-A
.ms_jumbotron.section-A {
   
    .ms_col {
        height: 100vh;
    }

    .ms_col.text {
        padding-top: 8rem;

        // Card-a
        .card-a {

            .title {
                font-size: 6rem;
                line-height: 7rem; 
            }
        }
    }
    .ms_col.image {
        position: relative;
        order: 2;
    
        .ms_overlay {
            height: 50%;
            background: linear-gradient(rgba(0, 0, 0, 0.9), #0000);
        }
    }
}
</style>

