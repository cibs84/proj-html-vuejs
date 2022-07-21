<template>
  <div id="app">
      <!-- Transfer linksArray to HeaderComponent for generating dynamic links -->
      <HeaderComponent :linksArray="headerLinks"/>
      
      <MainComponent :dataMenu="dataMenu" :visibleButtons="visibleButtons"/>

      <!-- Transfer socialsArray to FooterComponent for generating dynamic links -->
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
      ],
      dataMenu: [
        {
          course: 'HORS D’OEUVRES',
          dish: 'Ahi Salmon Nigiri',
          price: 48,
          description: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit lacinia.',
          url: '#'
        },
        {
          course: 'HORS D’OEUVRES',
          dish: 'Umi Masu Salad',
          price: 21,
          description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
          url: '#'
        },
        {
          course: 'HORS D’OEUVRES',
          dish: 'Temaki With Crab',
          price: 32,
          description: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'HORS D’OEUVRES',
          dish: 'California Rolls',
          price: 22,
          description: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'HORS D’OEUVRES',
          dish: 'Gamberi In Salsa Teriaki',
          price: 30,
          description: 'Cursus duis proin semper, senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'MAIN COURSE',
          dish: 'Braised Abalone',
          price: 52,
          description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
          url: '#'
        },
        {
          course: 'MAIN COURSE',
          dish: 'Twice Cooked Pork',
          price: 21,
          description: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'MAIN COURSE',
          dish: 'Kung Pao Chicken',
          price: 32,
          description: 'Quis duis sit dictum aliquam a velit enim. Tellus in sit augue aliquam.',
          url: '#'
        },
        {
          course: 'MAIN COURSE',
          dish: 'Char Siu & Sushis',
          price: 48,
          description: 'Feugiat rhoncus ipsum tristique purus diam, et dolor molestie.',
          url: '#'
        },
        {
          course: 'MAIN COURSE',
          dish: 'Brasato Di Manzo',
          price: 56,
          description: 'Felis massa vehicula tristique purus diam, et dolor molestie.',
          url: '#'
        },
        {
          course: 'DESSERTS',
          dish: 'Chocolate Ball Cake',
          price: 13,
          description: 'In pellentesque in felis massa vehicula. In sed euismod ut.',
          url: '#'
        },
        {
          course: 'DESSERTS',
          dish: 'Lime Pie With Crust',
          price: 14,
          description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
          url: '#'
        },
        {
          course: 'DESSERTS',
          dish: 'Raspberry Pear Cake',
          price: 18,
          description: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'DESSERTS',
          dish: 'Café Au Lait',
          price: 6,
          description: 'Ac vel, risus ornare senectus placerat duis amet dictumst tellus.',
          url: '#'
        },
        {
          course: 'DESSERTS',
          dish: 'Caffé con panna',
          price: 6,
          description: 'Modi tempora sequi sed dignissimos, necessitatibus voluptates.',
          url: '#'
        }
      ],
      visibleButtons: false
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
