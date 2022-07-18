<template>
    <main>
        <SectionJumbotron/>
        <SectionCorporateMessage/>
        <SectionBestTable/>
        <SectionReviews/>
        <SectionTakeout/>
    </main>
</template>


<script>
import SectionJumbotron from "./SectionJumbotron.vue";
import SectionBestTable from "./SectionBestTable.vue";
import SectionTakeout from "./SectionTakeout.vue";
import SectionCorporateMessage from "./SectionCorporateMessage.vue";
import SectionReviews from "./SectionReviews.vue";

export default {
    name: 'MainComponent',
    components: {
        SectionJumbotron,
        SectionCorporateMessage,
        SectionBestTable,
        SectionReviews,
        SectionTakeout,
    }
}
</script>


<style lang="scss" scoped>
@import '../assets/styles/variables.scss';


</style>