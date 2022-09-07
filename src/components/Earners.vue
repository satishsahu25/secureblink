<template>
    <div class="earn">
        <h3>Top Earners</h3>
        <h2>Transformng your ideas <br> into reality</h2>
        <div class="earners container">
            <div class="item">
                <img src="../assets/jonas-kakaroto-mjRwhvqEC0U-unsplash.png" alt="">
                <h4>Rs. 8,00,000</h4>
            </div>
            <div class="item">
                <img src="../assets/christopher-campbell-rDEOVtE7vOs-unsplash.png" alt="">
                <h4>Rs. 6,00,000</h4>
            </div>
            <div class="item">
                <img src="../assets/craig-mckay-jmURdhtm7Ng-unsplash.png" alt="">
                <h4>Rs. 5,00,000</h4>
            </div>
            <div class="item">
                <img src="../assets/luis-villasmil-hh3ViD0r0Rc-unsplash.png" alt="">
                <h4>Rs. 4,50,000</h4>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .earners{
        display: flex;  
    }
        .earn h3{
        font-style: italic;
        font-weight: normal;
        font-size: 20px;
        margin-left: 10rem;
        color:#01CB63;
    }
    .earners div{
        margin: 0.5rem 1rem;
        flex: 1;  
    }
    .earn h2{
        margin-left: 10rem;
        font-weight: 500;
        margin-bottom: 5rem;
    }
   
    .earners .item h4{
        padding: 0.2rem;
        margin-top: 0.5rem;
        font-weight: bold;
        border-left: 5px solid #01CB63;
    }
    .earners .item{
        flex: 1;
    }
    .earners .item img{
       height:15rem;
       width:12rem;
       border-radius: 10px;
        object-fit: cover;
    }
    
@media only screen and (max-width:1200px){
    .earners{
        align-items: center;
        flex-wrap: wrap;
    }
  
  
}
@media only screen and (max-width:760px){
    .earners .item{
        display: flex;
        flex-direction: column;
      align-items: center;
    }
    .earn h2{
        margin-left: 0;
        text-align: center;
    }
    .earn h3{
        margin-left: 0;
        text-align: center;
    }
}

</style>