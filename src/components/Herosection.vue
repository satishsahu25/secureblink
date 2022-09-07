<template>
    <div class="hero">
        <div class="lefth">
            <div class="content">
                <h1>
                    AnyTime, Anywhere <br> Learn on your schedule<br> from any device
                </h1>
                <p>
                    We Believe everyone has the capcity to be creative <br>
                     <span>Course Pro</span>
                     is a place where people develop their <br> own potential
                </p>
                <button class="startbtn">Let's Get Start</button>
            </div>
        </div>
        <div class="righth">
                <img src="../assets/herogirl.jpg" alt="">
        </div>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .hero{
        display: flex;
        margin-top: 1rem;
    }
    .lefth{
        background-color: #01CB63;
        flex: 1;
        padding:5rem;
    }
    .lefth h1{
        color: white;
    }
    .lefth .content h1{
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;

    }
    .lefth .content p{
        font-size: 20px;       
    }
    .lefth p>span{
        color: white;
        font-weight: 600;
    }
    .lefth button{
        background-color: black;
        border: none;
        outline:none;
        color: white;
        border-radius: 5px;
        padding: 0.5rem 1rem;
        font-style: italic;
    }
    .righth{
        flex: 1;
    }
    .righth img{
        object-fit: cover;
        height: 100%;
        width:100%;
    }

    /* responsiveness */
    @media only screen and (max-width: 1200px) {
        .hero{
            flex-direction:column-reverse;

        }
}


</style>