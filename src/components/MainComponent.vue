<template>
    <section class="ms_jumbotron">
        <div class="ms_col text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eligendi, voluptate laboriosam impedit mollitia cumque aperiam magni quisquam, illum id dolores dolorem non cum minus in. Error numquam quia veniam laudantium!
        Officia dolorem quod esse temporibus quae amet harum laboriosam blanditiis autem quas debitis earum distinctio libero numquam, voluptate beatae ipsam quibusdam ea rerum unde totam nam. Neque necessitatibus ea hic.
        Ipsum nobis rerum velit odio veritatis soluta ab exercitationem eaque dolore! Quae, minus! Eius, vero provident. Inventore pariatur repellendus nulla ab ipsum maiores exercitationem eligendi distinctio facere, ipsam tempore velit.</div>
        
        <div class="ms_col image">
            <img src="../assets/img/slider52x.jpg" alt="">
        </div>
    </section>
</template>


<script>
export default {
    name: 'MainComponent'
}
</script>


<style lang="scss" scoped>
.ms_jumbotron {
    // position: absolute;
    // top: 0;
    // left: 0;
    display: flex;
    justify-content: space-between;

    .ms_col {
    border: 1px solid red;
    height: 100vh;
    }
    .ms_col.text {
        width: 40%;
        background-color: black;
        padding: 10rem 7.5%;
        color: white;
    }
    .ms_col.image {
        width: 60%;
        background-color: lightcoral;

        img {
            width: 100%;
            object-fit: cover;
        }
    }
    
}
</style>