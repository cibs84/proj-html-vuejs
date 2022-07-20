<template>
    <section class="dish-banner">
        <div class="ms_secondary_container">
            <!-- Column -->
            <div class="ms_col">
                <!-- Card-b - A random dish from the dataMenu array -->
                <div class="card-b">
                    <!-- Dish, Price and Description -->
                    <h3 class="dish">{{this.randomDish.dish}}</h3>
                    <div class="price">${{this.randomDish.price}}</div>
                    <div class="line-separator"></div>
                    <p>{{this.randomDish.description}}</p>
                    <!-- Button -->
                    <a :href="randomDish.url">View in the menu</a>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionPhotoBanner',
    props: {
        dataMenu: Array
    },
    methods: {
        // Returns a random number between min and max (both included)
        getRndInteger(min, max) {
            return Math.floor(Math.random() * (max - min + 1) ) + min;
        }
    },
    computed: {
        // Returns a random item from dataMenu array
        randomDish(){
            const rndIndex = this.getRndInteger(0, this.dataMenu.length-1);
            return this.dataMenu[rndIndex]
        }
    }
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
                    
                .dish {
                    display: inline-block;
                    max-width: 87%;
                    margin-bottom: 3.5rem;
                    font-size: 4.5rem;
                    font-weight: 400;
                
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