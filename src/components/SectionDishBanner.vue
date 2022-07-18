<template>
    <section class="dish-banner">
        <div class="ms_secondary_container">
            <!-- Column -->
            <div class="ms_col">
                <!-- Card-b -->
                <div class="card-b">
                    <h3 class="title">Braised Abalone</h3>
                    <div class="price">$52</div>
                    <div class="line-separator"></div>
                    <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
                    <!-- Button -->
                    <a href="#">View in the menu</a>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionPhotoBanner'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.dish-banner {
    padding: 8rem 0;
    background-image: url('../assets/img/hero42x.jpg');
    background-size: cover;

    .ms_secondary_container {

        .ms_col {
            width: 40%;
            background-color: $ms_black;
            padding: 5rem;
    
            .card-b {
            flex-direction: column;
            align-items: flex-start;
            position: relative;
    
                .title {
                    margin-bottom: 3.5rem;
                    width: 30%;
                    font-size: 4.5rem;
                }
                .price {
                    position: absolute;
                    right: 0;
                    top: 1rem;
                    font-size: 1rem;
                    letter-spacing: 0.1rem;
                }
            }
        }
    }
}
</style>