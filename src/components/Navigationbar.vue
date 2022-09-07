<template>
<nav>
    <div class="logo">
        <img src="../assets/mainlogo.svg" alt="">
    </div>
    <input type="checkbox" id="click">
    <label for="click" class="menubtn">
        <i class="fas fa-bars"></i>
    </label>
    <ul>
        <li class="logbtn">Login</li>
        <li class="regbtn">Register</li>
    </ul>
</nav>

</template>

<script>
export default {};
</script>
<style scoped>
   *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
   }
   nav{
    position: fixed;
    top: 0;
    width: 100%;
    background: white;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0px 50px 0px 100px;
   }
   nav i{
    color: black;
   }
   nav .menubtn{
    color: #fff;
    display: none;
    font-size: 22px;
    cursor: pointer;
   }
   nav ul{
    display: flex;
    list-style: none;
   }
   nav ul li {
    margin: 0 5px;
    letter-spacing: 1px;
    padding: 8px 10px;
    text-decoration: none;
   }
   nav .regbtn{
    color: white;
    background-color: #01CB63;
    border-radius: 5px;
   }

   #click{
    display: none;
   }
   @media (max-width:940px){
    nav .menubtn{
        display: block;
    }
    nav ul{
        transition:  all 0.3s ease;
        position: fixed;
        top: 50px;
        left: -100%;
        height: 100vh;
        width: 100%;
        background-color: rgba(255, 255, 255, 0.774);
        display: block;
        text-align: center;
    }
    #click:checked~ul{
    left: 0%;
   }
    nav ul li{
        margin: 10px 0;
        font-weight: bold;
        font-size: 22px;
        font-family: "";
    }
    nav .regbtn{
    color: black;
    background-color: transparent;
   }
    nav ul li:hover{
        text-decoration: underline;
        cursor: pointer;
    }
   }

</style>
