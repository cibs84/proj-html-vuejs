<template>
    <section class="restaurant-menu">
        <div class="ms_container">

            <!-- Column Left -->
            <div class="ms_col">
                <!-- Card -->
                <div class="ms_card">
                    <h3 class="title">HORS D’OEUVRES</h3>

                    <!-- List -->
                    <ul class="list">
                        <!-- Item List -->
                        <li class="item-list" v-for="(iteration, index) in 4" :key="index">
                            <div class="item-heading">
                                <h4 class="dish">{{menuAppetizer[index].dish}}</h4>
                                <span class="price">${{menuAppetizer[index].price}}</span>
                            </div>
                            <p class="description">{{menuAppetizer[index].description}}</p>
                        </li>
                    </ul>
                </div>
            </div>

            <!-- Column Middle -->
            <div class="ms_col middle">
                <div class="ms_overlay"></div>
                 <!-- Card -->
                <div class="ms_card">
                    <h3 class="title">Main Course</h3>
                    
                    <!-- List -->
                    <ul class="list">
                        <!-- Item List -->
                        <li class="item-list" v-for="(iteration, index) in 4" :key="index">
                            <div class="item-heading">
                                <h4 class="dish">{{menuMainCourse[index].dish}}</h4>
                                <span class="price">${{menuMainCourse[index].price}}</span>
                            </div>
                            <p class="description">{{menuMainCourse[index].description}}</p>
                        </li>
                    </ul>
                </div>
            </div>
            

            <!-- Column Right -->
            <div class="ms_col">
                 <!-- Card -->
                <div class="ms_card">
                    <h3 class="title">DESSERTS</h3>

                    <!-- List -->
                    <ul class="list">
                        <!-- Item List -->
                        <li class="item-list" v-for="(iteration, index) in 4" :key="index">
                            <div class="item-heading">
                                <h4 class="dish">{{menuDesserts[index].dish}}</h4>
                                <span class="price">${{menuDesserts[index].price}}</span>
                            </div>
                            <p class="description">{{menuDesserts[index].description}}</p>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionMenu',
    props: {
        dataMenu: Array
    },
    computed: {
        // dataMenu filtered by course property
        menuAppetizer(){
            return this.dataMenu.filter(element => {
                return element.course === 'HORS D’OEUVRES'
            });
        },
        menuMainCourse(){
            return this.dataMenu.filter(element => {
                return element.course === 'MAIN COURSE'
            });
        },
        menuDesserts(){
            return this.dataMenu.filter(element => {
                return element.course === 'DESSERTS'
            });
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.restaurant-menu {
    padding: 11rem 0 8rem;

    .ms_container {
        display: flex;

        .ms_col {
            height: 57rem;
            background-color: #e8e8e8;
            width: calc(100% / 3);

            .ms_card {
                height: 100%;
                padding: 6rem;

                .title {
                    text-transform: uppercase;
                    margin-bottom: 3rem;
                    font-size: 2.8rem;
                    font-weight: 500;
                }

                .list {

                   .item-list {
                        margin-bottom: 2.5rem;

                        .item-heading {
                            display: flex;
                            justify-content: space-between;
                            align-items: baseline;
                            
                            .dish {
                            display: inline-block;
                            text-transform: uppercase;
                            font-size: 2rem;
                            font-weight: 500;
                            font-family: 'Bebas Neue', Arial, Helvetica, sans-serif;

                            }
                            .price {
                                text-transform: uppercase;
                                font-size: 1rem;
                                letter-spacing: 0.1rem;
                                font-weight: 600;
                            }
                            .description {
                                line-height: 2rem;
                                font-size: 1.2rem;
                                margin-top: 0.5rem;
                            }
                        }
                        
                   } 
                }
            }
        }
        .ms_col.middle {
            position: relative;
            top: -3rem;
            background-image: url('../assets/img/misc22x.jpg');
            background-size: cover;
            background-position: bottom;

            .ms_card {
                position: relative;
                color: white;
            }
        }
    }
}
</style>