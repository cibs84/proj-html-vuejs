<template>
    <footer>
        <!-- Footer Top -->
        <div class="footer-top">
            <div class="overlay"></div>
            <!-- Content -->
            <div class="content">
                <img src="../assets/img/logo-restaurant-2x-300x58.png" alt="Avada Logo" class="logo">
                <p>Phasellus molestie pellentesque mi quis lobortis. Mauris convallis quam tincidunt nunc interdum, porttitor lacinia nibh.</p>
                <!-- Social Links -->
                <ul class="social-links">
                    <li>
                        <a href="#">
                            <span><i class="fa-brands fa-circle fa-facebook-f"></i></span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <span><i class="fa-brands fa-circle fa-twitter"></i></span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <span><i class="fa-brands fa-circle fa-youtube"></i></span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <span><i class="fa-brands fa-circle fa-instagram"></i></span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <span><i class="fa-brands fa-circle fa-linkedin-in"></i></span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <!-- Footer Bottom -->
        <div class="footer-bottom">
            © Copyright 2012 - 2019 Avada | All Rights Reserved | Powered by <a href="#">WordPress</a> | <a href="#">ThemeFusion</a>
        </div>
    </footer>
</template>


<script>
export default {
    name: 'FooterComponent'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

footer {
    // Footer Top
    .footer-top {
        display: flex;
        justify-content: center;
        align-items: center;
        background-image: url('../assets/img/footer2x.jpg');
        background-size: cover;
        background-position: center;
        height: 40rem;
        position: relative;

        .content {
            width: 30%;
            text-align: center;

            .logo {
            width: 19rem;
            margin-bottom: 3rem;
            }
            p {
                color: white;
                margin-bottom: 3rem;
                font-size: 1.2rem;
                line-height: 2rem;
                text-transform: initial;
                font-family: 'Lora', Arial, Helvetica, sans-serif;
                font-weight: 400;
                margin-bottom: 3.5rem; 
            }
            .social-links {
                display: flex;
                justify-content: center;
                align-items: center;
                color: $ms_black;

                span {
                    background-color: white;
                    display: inline-block;
                    width: 3rem;
                    height: 3rem;
                    border-radius: 50%;
                    text-align: center;
                    line-height: 3rem;
                    margin-right: 0.5rem;
                    transition: 0.3s;

                    &:hover {
                        background-color: $ms_silver;
                        color: white;
                    }
                }

            }
        }
    }

    // Footer Bottom
    .footer-bottom {
        text-align: center;
        font-size: 0.7rem;
        color: white;
        font-family: 'Lora', Arial, Helvetica, sans-serif;
        background-color: $ms_black;
        padding: 2rem 0;
        color: $ms_silver;

        a {
            font-weight: 500;
            transition: 0.3s;
            color: white;

            &:hover {
                color: $ms_silver;
            }
        }
    }
}
</style>