<template>
    <div class="courses container">
        <h3>Courses</h3>
        <h2>Our Most Popular Courses</h2>
        <div class="coursecontent">
            <Courseitem
             v-for="course in coursedata"
              :key="course.id"
              :course="course"
              />
         
        </div>

    </div>
</template>

<script>
import Courseitem from './Courseitems/Courseitem.vue';
import {coursedata} from '../../src/data.js'    
export default {
    components: { Courseitem },
    data(){
        return {
            coursedata:coursedata
        }
    }
}
</script>

<style scoped>
    .courses{
        margin-top: 5rem;
        margin-bottom: 5rem;
    }
    .courses h3{
        text-align: center;
        font-style: italic;
        font-weight: normal;
        font-size: 20px;
        color:#01CB63;
    }
    .courses h2{
        text-align: center;
    }
    .coursecontent{
        display: flex;
        padding-top: 2rem;
    }

@media only screen and (max-width:1200px) {
     .coursecontent{
        flex-direction: column;
    }
    
}
</style>