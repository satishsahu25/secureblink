<template>
  <div class="app">
    <Navigationbar/>
    <Herosection/>
    <Numbers/>
    <Courses/>
    <Earners/>
    <Refer/>
    <Testimonials/>
    <Contactus/>
    
  </div>
</template>

<script>
import Navigationbar from './components/Navigationbar.vue';
import Herosection from './components/Herosection.vue';
import Courses from './components/Courses.vue';
import Refer from './components/Refer.vue';
import Testimonials from './components/Testimonials.vue';
import Numbers from './components/Numbers.vue';
import Contactus from './components/Contactus.vue';
import Earners from './components/Earners.vue';


  export default {
    components: { Navigationbar, Herosection, Courses, Refer, Testimonials, Numbers, Contactus, Earners }
}
</script>

<style scoped>
.app{
  margin: 0;
  padding: 0;
  overflow: hidden;
}

</style>