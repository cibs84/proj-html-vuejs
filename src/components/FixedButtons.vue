<template>
    <div>
        <!-- Demos Button -->
        <button class="demos-button btn">
            <!-- Icon -->
            <span class="demos-icon">
                <i class="fa-brands fa-buffer"></i>
            </span>

            <!-- Text\ -->
            <div class="text">Demos</div>
        </button>


        <!-- Sales Button -->
        <button class="sales-button btn">
            <!-- Price -->
            <div class="price">
                <sup>$</sup>39
            </div>

            <!-- Text -->
            <div class="text">On Sale</div>
        </button>


        <!-- Up Button -->
        <a href="#">
            <span class="up-button">
                <i class="fa-solid fa-angle-up"></i>
            </span>
        </a>
    </div>
</template>

<script>
export default {
    name: 'FixedButtons'
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.btn {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 4.1rem;
    height: 4.1rem;
    top: 10rem;
    right: 1rem;
    position: fixed;
    z-index: 100;

    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    cursor: pointer;
    background-color: #fff;
    border-radius: 6px;
    color: #6f7f8c;
    border-color: #00000047;
    
    .text {
       font-size: 0.8rem;
       font-weight: 600;
    }
}
.demos-button {

    .demos-icon {
        color: #6f7f8c;
        z-index: 1000;
        font-size: 2rem;
    }
}
.sales-button {
    top: 14.5rem;

    .price {
       color: #69a10e;
       font-size: 1.5rem;
       font-weight: 600;
    }
}
.up-button {
    background-color: #2e2e2d;
    bottom: 0px;
    display: block;
    height: 35px;
    position: fixed;
    right: 75px;
    width: 48px;
    z-index: 100000;

    font-size: 1.2rem;
    text-align: center;
    line-height: 2.4rem;
    color: white;
}
</style>

