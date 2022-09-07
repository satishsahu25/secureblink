<template>
    <div class="course">
        <div class="main">
            <img src="https://res.cloudinary.com/codercloud/image/upload/v1662458672/download_1_wqnwxr.jpg" alt="">
            <div class="type">{{course.coursetype}}</div>
        </div>
        <div class="title">{{ course.coursetitle }}</div>
       <p><span>{{course.registeredstudents}}</span>Students</p>
        <div class="desc">
            <div class="timeremain">
                <img src="../../assets/schedule-24px.svg" alt="">
                <span>17 hr 20 min</span>
            </div>
            <div class="totallectures">
                <img src="../../assets/date_range-24px.svg" alt="">
                <span>{{course.totallectures}} Lectures</span>
            </div>
        </div>
        <hr>
        <div class="price">
            <div class="teacher">
                <img src='../../assets/jonas-kakaroto-mjRwhvqEC0U-unsplash.png' alt="">
                <span>{{course.teacher}}</span>
            </div>
            <div class="discount">
                <div class="newprice">Rs.{{course.newprice}}</div>
                <div class="oldprice">Rs.{{course.oldprice}}</div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        // to recieve props we have to tell
        
        
        props:{
            course:{
                type:Object,
                required:true
            },
            
        }
        
    }
</script>

<style scoped>
    .course{
        flex: 1;
        margin:1rem;
        border: 1px solid #E6E6E6;
        border-radius: 15px 15px 0px 0px;
    }
    .course hr{
        color: #b6b4b4;
    }
    .main{
        position: relative;
    }
    .course .main div{
        position: absolute;
        bottom: 1rem;
        right: 1rem;
    }
    .type{
        background-color: black;
        border: none;
        border-radius: 5px;
        color: #01CB63;
        font-style: italic;
        padding: 0.2rem 1rem;
    }
    .course .title{
        font-size: 20px;
        font-weight: 500;
        padding: 0.2rem;
    }
    .main img{
        object-fit: cover;
        height: 15rem; 
        width: 100%;
        border-radius: 15px 15px 0px 0px;
    }
    .course span{
        font-weight: 600;
        padding: 0.5rem 1rem;
        font-size: 20px;
    }
    .course p span{
        font-weight: bold;
    }
    .registeredstudents span{
        font-weight: bold;
    }
    .desc{
        justify-content: space-between;
        display: flex;
        align-items: center;
        font-size: 20px;
        font-weight: normal;
        font-style: italic;
        color: #86919D;
        padding: 0.5rem;
        margin-top: -1rem;
        margin-bottom: -1rem;
    }
    .desc .timeremain{
        display: flex;
        align-items: center;
        font-size: 10px;
    }
    .desc .timeremain span{
        font-size: 18px;
    }
    .desc .totallectures{
        display: flex;
        align-items: center;
    }
    .desc .totallectures span{
        font-size: 18px;
    }
    .price{
        display: flex;
        align-items: center;
        justify-content: space-between;
         font-size: 18px;
         padding: 0.5rem;
    }
    .price .teacher {
        display: flex;
        align-items: center;
        
    }
    .price .teacher span{
        font-size: 15px;
    }
    .price .teacher img{
        height: 2rem;
        width: 2rem;
        border-radius: 50%;
    }
    .price .discount{
        margin: 0.2rem;
        display: flex;
        align-items: center;
    }
    .price .discount .newprice{
        color: #01CB63;
        font-weight: 500;
        font-size: 22px;
    }
    .price .discount .oldprice{
        font-weight: 500;
        text-decoration: line-through;
        margin-left: 0.1rem;
        font-size: 18px;
    }
</style>