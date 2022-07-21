<template>
    <main>
        <SectionJumbotron/>
        <SectionCorporateMessage/>
        <SectionFeatures/>
        <SectionBestTable/>
        <SectionReviews/>
        <SectionPhotoBanner/>
        <SectionNewsPromotion/>
        <SectionTakeout/>
        <SectionMenu :dataMenu="dataMenu"/>
        <SectionDishBanner :dataMenu="dataMenu"/>

        <FixedButtons :visibleButtons="visibleButtons"/>

    </main>
</template>


<script>
import SectionJumbotron from "./SectionJumbotron.vue";
import SectionBestTable from "./SectionBestTable.vue";
import SectionTakeout from "./SectionTakeout.vue";
import SectionCorporateMessage from "./SectionCorporateMessage.vue";
import SectionReviews from "./SectionReviews.vue";
import SectionPhotoBanner from "./SectionPhotoBanner.vue";
import SectionDishBanner from "./SectionDishBanner.vue";
import SectionMenu from "./SectionMenu.vue";
import SectionFeatures from "./SectionFeatures.vue";
import SectionNewsPromotion from "./SectionNewsPromotion.vue";
import FixedButtons from "./FixedButtons.vue";

export default {
    name: 'MainComponent',
    components: {
        SectionJumbotron,
        SectionCorporateMessage,
        SectionBestTable,
        SectionReviews,
        SectionTakeout,
        SectionPhotoBanner,
        SectionDishBanner,
        SectionMenu,
        SectionFeatures,
        SectionNewsPromotion,
        FixedButtons
    },
    props: {
        dataMenu: Array,
        visibleButtons: Boolean
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';


</style>