<template>
    <div class="refer">
        <h3>Refer</h3>
        <h2>How It's Work</h2>
        <img src="../assets/refer.svg" alt="">

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .refer{
        margin-top: 8rem;
    }
    .refer h3{
        font-style: italic;
        font-weight: normal;
        font-size: 20px;
        color:#01CB63;
        margin-left: 10rem;
    }
    .refer h2{
        margin-left: 10rem;
        font-weight: 500;
    }
    .refer img{
        width: 100%;
        object-fit: cover;
        height:auto;
    }
    @media only screen and (max-width:960px){
        .refer h2{
        margin-left: 0;
        text-align: center;
    }
    .refer h3{
        margin-left: 0;
        text-align: center;
    }
    }

</style>