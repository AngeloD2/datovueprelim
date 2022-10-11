<template>
  <!-- use components here -->
  <div id="app"> 
    <nav-bar> </nav-bar>
    <!-- Introduction -->
    <hom-e id="home" 
    greetings="Hello! I am"
    name="Angelo Dato"
    title="Full Stack Developer"
    desc="I am a Fourth Year Information Technology Student from La Consolacion College Bacolod.
    Got an idea? Let's get started!" 
    />
    <!-- Skills -->
    <skill-s id="skills"> </skill-s>
  
    <!-- Portfolio / Sample Works -->
    <PortFolio id="portfolio"> </PortFolio>
    
    <!-- Contact -->
    <contac-t id="contact"
      mobile="+63 976 004 4715"
      landline="+434 9874"
      email="angelodato@rocketmail.com" />
      <FooTer />


  </div>
</template>


<!-- import components here -->
<script>

import NavBar from './components/navbar.vue'
import homE from './components/home.vue'
import SkillS from './components/skills.vue'
import PortFolio from './components/sampleworks.vue'
import contacT from './components/contact.vue'
import FooTer from './components/footer.vue'

export default {
  name: 'App',
  components: {
    homE,
    NavBar,
    SkillS,
    PortFolio,
    contacT,
    FooTer
}
}
</script>

