<template>
  <div class="testimonials container">
    <h3>Testimonials</h3>
    <h2>
      Check out What Our
      <br />
      Students Think About Us
    </h2>
    <div class="testimonial">
        <Testitems 
        v-for="test in testdata"
         :key="test.id"
         :testit="test"
        />
      
    </div>
  </div>
</template>

<script>
import Testitems from './Testimonials/testitems.vue';
import {testdata} from '../../src/testdata.js'
export default {
   components: { Testitems } 
   ,
   data(){
    return{
      testdata:testdata
    }
   }
};
</script>

<style scoped>
 
    .testimonials h3{
        font-style: italic;
        font-weight: normal;
        font-size: 20px;
        color:#01CB63;
    }
    .testimonials h2{
        font-weight: 600;
        font-size: 25px;
        margin-bottom: 3rem;
    }
.testimonial{
    display: flex;
    margin: 1rem;
    padding: 2rem;

}
@media only screen and (max-width:1200px){
  .testimonial{
    flex-direction: column;
  }
  
}
@media only screen and (max-width:960px){
        .testimonials h2{
        margin-left: 0;
        text-align: center;
    }
    .testimonials h3{
        margin-left: 0;
        text-align: center;
    }
    }

</style>
