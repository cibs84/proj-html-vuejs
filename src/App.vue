<template>
  <div id="app">
      <!-- Transfer linksArray to HeaderComponent for generating dynamic links -->
      <HeaderComponent :linksArray="headerLinks"/>
      <MainComponent />
      <FooterComponent :socialsArray="footerSocialLinks"/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
      HeaderComponent,
      MainComponent,
      FooterComponent
  },
  data() {
    return {
      headerLinks: [
        {
          title: 'Home',
          url: '#',
          label: null
        },
        {
          title: 'Culinary History',
          url: '#',
          label: null
        },
        {
          title: 'Our Team',
          url: '#',
          label: null
        },
        {
          title: 'Our Menu',
          url: '#',
          label: null
        },
        {
          title: 'Takeout',
          url: '#',
          label: 'New'
        },
        {
          title: 'Bulletin',
          url: '#',
          label: null
        },
        {
          title: 'Reservations',
          url: '#',
          label: null
        }
      ],
      footerSocialLinks: [
        {
          name: 'Facebook',
          url: '#',
          class: 'fa-facebook-f'
        },
        {
          name: 'Twitter',
          url: '#',
          class: 'fa-twitter'
        },
        {
          name: 'Youtube',
          url: '#',
          class: 'fa-youtube'
        },
        {
          name: 'Instagram',
          url: '#',
          class: 'fa-instagram'
        },
        {
          name: 'Linked-In',
          url: '#',
          class: 'fa-linkedin-in'
        }
      ]
    }
  },
  mounted() {
    // DEBUG
    console.log('headerLinks: ', this.headerLinks);
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';
@import './assets/styles/variables.scss';
</style>
