<template>
  <v-app dark>
    <header class="header">
      <div class="logo">
        <img src="/logoblanc.png" alt="logo">
      </div>
      <nav class="ancres">
        <a href="#home">Home</a>
        <a href="#presentation">Presentation</a>
        <a href="#">Skills</a>
        <a href="#">Works</a>
        <a href="#">Contact</a>
      </nav>
        
    </header>
    
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>


    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<style lang="scss">
.v-application a {
text-decoration: none;
  color: #fff;
}
html{
  scroll-behavior: smooth;
}
section{
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    top: 6rem;
}
.header{
    width: 100vw;
    padding: 0 5vw;
    top: 50px;
    display: flex;
    justify-content: space-between;
    position: fixed;
    align-items: center;
    z-index: 100;
  .logo{
        height: 11rem;
    width: 11rem;
    img{
      width: 100%;
      height: 100%
      ;
    }
  }

}

nav{
    display: flex;
    justify-content: space-evenly;
    width: 47vw;
    a{
        text-transform: uppercase;
        
    }
}

</style>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'portfolio',
          to: '/portfolio'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
