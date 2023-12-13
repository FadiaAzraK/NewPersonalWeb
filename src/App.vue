<template>
  <Navbar></Navbar>
  <Home></Home>
  <br>
  <about></about>
  <portofolio></portofolio>
  <contact></contact>
  <Footer></Footer>
</template>
<script>
import Navbar from '@/components/Layouts/Navbar.vue';
import Home from '@/pages/Home.vue';
import about from '@/components/about/about.vue'
import Footer from '@/components/Layouts/Footer.vue';
import portofolio from '@/components/portofolio/portofolio.vue';
import contact from '@/components/contact/contact.vue';
export default {
  components: {
    Navbar,
    Footer,
    Home,
    about,
    portofolio,
    contact
  },
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');

  *{
    font-family: 'Poppins', sans-serif;
  }

</style>