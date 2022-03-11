<template>
<Navbar/>
<Home/>
<About/>
<Skills/>
<Projects/>
<Testimonials/>
<Contact/>


</template>

<script>
import Home from './components/Home.vue'
import About from './components/About.vue'
import Navbar from './components/Navbar'
import Skills from './components/Skills' 
import Testimonials from './components/Testimonials.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Home,
    About,
    Navbar,
    Skills,
    Testimonials,
    Projects,
    Contact 
  }
}

</script>

<style>

#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}





</style>
