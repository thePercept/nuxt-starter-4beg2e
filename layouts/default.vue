<template>
  <div>
    <LoadSpinner v-if="showHideSpinner" />
    <CThemeProvider>
      <CColorModeProvider>
        <CBox font-family="body" as="main">
          <CReset />
          <siteHeader />
          <nuxt />
        </CBox>
      </CColorModeProvider>
    </CThemeProvider>
  </div>
</template>
<script>

import siteHeader from '../components/siteHeader.vue';


export default {
  name: 'App',

  head() {
    return {
      title: 'AN Corp PVT Ltd',

      link: [
        { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' },
        { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
        {
          rel: 'preconnect',
          href: 'https://fonts.gstatic.com',
          crossorigin: '',
        },
        {
          rel: 'stylesheet',
          href: 'https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200&display=swap',
        },
      ],
    };
  },
  beforeCreate() {
    this.showHideSpinner = true;
  },

  mounted() {
    this.showHideSpinner = false;
  },

  computed: {

  },

  beforeDestroy() {
  },

  data() {
    return {
      showHideSpinner: true,
    };
  },

  methods: {



  },

  components: {
    siteHeader
  },
};
</script>
<style>
html,
h1,
h2,
h3,
h4,
p {
  font-family: 'Montserrat', sans-serif !important;
}
body {
  background-color: #f4f4f4;
}
#__nuxt {
  overflow-y: hidden;
}

.home-enter-active,
.home-leave-active {
  transition: opacity 0.5s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}

.view-all-link {
  text-decoration: underline;
}
</style>
