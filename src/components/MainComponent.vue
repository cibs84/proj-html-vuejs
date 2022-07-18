<template>
    <main>
        <SectionJumbotron/>
        <SectionCorporateMessage/>
        <SectionBestTable/>
        <SectionReviews/>
        <SectionPhotoBanner/>
        <SectionTakeout/>
    </main>
</template>


<script>
import SectionJumbotron from "./SectionJumbotron.vue";
import SectionBestTable from "./SectionBestTable.vue";
import SectionTakeout from "./SectionTakeout.vue";
import SectionCorporateMessage from "./SectionCorporateMessage.vue";
import SectionReviews from "./SectionReviews.vue";
import SectionPhotoBanner from "./SectionPhotoBanner.vue";

export default {
    name: 'MainComponent',
    components: {
        SectionJumbotron,
        SectionCorporateMessage,
        SectionBestTable,
        SectionReviews,
        SectionTakeout,
        SectionPhotoBanner
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';


</style>