<template>
    <!-- HEADER -->
    <header>
        <div class="ms_container">
            <!-- Logo -->
            <a href="#">
                <img src="../assets/img/logo-restaurant-2x-300x58.png" alt="Avada restaurant logo" class="logo">
            </a>
            
            <!-- Main Menu -->
            <nav class="main-menu">
                <ul>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>
                    <li><a href="#">My Link</a></li>

                    <!-- Cart Icon -->
                    <li class="icon-cart">
                        <a href="#"><i class="fas fa-shopping-cart"></i></a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>


<script>
export default {
    name: 'HeaderComponent'
}
</script>


<style lang="scss" scoped>
header {
    background-color: black;
    padding: 2.5rem 0;

    .ms_container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .main-menu {
            width: 50%;

            ul {
                display: flex;
                justify-content: space-between;

                li {
                    color: #c0c0c0;
                    font-weight: 600;

                    a:hover {
                        color: white;
                    }
                }
            }
        }

    }
}
</style>