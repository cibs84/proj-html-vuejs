<template>
    <main>
        <SectionJumbotron/>
        <SectionCorporateMessage/>
        <SectionBestTable/>
        <SectionReviews/>
        <SectionPhotoBanner/>
        <SectionTakeout/>
        <SectionDishBanner/>
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
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';


</style>