<template>
    <!-- SECTION-A - The Best Table in Town -->
    <section class="corporate-message section-B">
        <div class="ms_secondary_container">

             <!-- Col Text -->
            <div class="ms_col text">
                <p>
                    <span class="text-uppercase fw-bold">HAC TELLUS, FELIS RISUS AT</span> 
                    mattis mattis. Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etiam duis facilisis amet vulputate.
                </p>
                <h2 class="title">food is our common ground, a universal experience.</h2>
                <p>
                    Tristique tempus condimentum diam donec. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.
                </p>
                <img src="../assets/img/signature-200x172.jpg" alt="">
            </div>
            
            <!-- Col Image -->
            <div class="ms_col image">
                <img src="../assets/img/info22x.jpg" alt="">
                <div class="overlay"></div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionCorporateMessage'
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

.section-B.corporate-message {
    padding: 8rem 0;
    
    .ms_col.text {
        background-color: white;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-end;
        color: $ms_black;
        width: 42%;
        padding: 0;

        .title {
            font-family: 'Bebas Neue', Arial, Helvetica, sans-serif;
            font-size: 4.5rem;
            font-weight: 400;
            line-height: 5.5rem; 
            margin-bottom: 2.5rem;
            text-transform: uppercase;
        }
        p {
            font-size: 1.2rem;
            line-height: 2rem;
            text-transform: initial;
            font-family: 'Lora', Arial, Helvetica, sans-serif;
            font-weight: 400;
            margin-bottom: 3rem;
        }
        img {
            width: 11rem;
        }
    }
    .ms_col.image {
        width: 47%;
        flex-shrink: 0;
    }
}
</style>