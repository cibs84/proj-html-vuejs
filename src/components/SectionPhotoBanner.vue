<template>
    <section class="photo-banner">
        <img src="../assets/img/page52x.jpg" alt="Kung Pao Chicken">
        <h6 class="price"><a href="#">Kung pao chicken - $32</a></h6>
    </section>
</template>


<script>
export default {
    name: 'SectionPhotoBanner'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.photo-banner {
    position: relative;

    img {
        width: 100%;
        height: 43.5rem;
        object-fit: cover;
        font-weight: 400;
    }
    .price {
        color: white;
        text-transform: uppercase;
        text-align: center;
        position: absolute;
        bottom: 1.5rem;
        left: 50%;
        transform: translate(-50%);
        font-size: 1rem;
        letter-spacing: 0.1rem;
    }
}
</style>