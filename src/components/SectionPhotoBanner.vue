<template>
    <section class="banner">
        <img src="../assets/img/page52x.jpg" alt="Kung Pao Chicken">
        <h6 class="price">Kung pao chicken - $32</h6>
    </section>
</template>


<script>
export default {
    name: 'SectionPhotoBanner'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.banner {
    position: relative;

    img {
        width: 100%;
        height: 43.5rem;
        object-fit: cover;
        font-weight: 400;
    }
    .price {
        font-size: 0.8rem;
        color: white;
        text-transform: uppercase;
        text-align: center;
        position: absolute;
        bottom: 3rem;
        left: 50%;
        transform: translate(-50%);
        font-size: 1rem;
        letter-spacing: 0.1rem;
    }
}
</style>