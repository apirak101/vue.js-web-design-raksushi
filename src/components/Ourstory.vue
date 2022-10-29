<template>
<div class="c-story reveal" id="ourstory">
    <div class="text-left">
        <p class="title-head">ourstory</p>
        <h1>OUR STORY</h1>
        <h2>✻</h2>
        <span>Rak Sushi is an authentic Japanese restaurant located in the heart of beautiful Lake Ridge Virginia. We
            are passionate about finding the freshest ingredients to craft the best tastes possible.</span><br><br>
        <p><a href="#ourstory" class="about">ABOUT US</a></p>
    </div>
    <div class="img-right reveal">
        <div class="img-story">
            <img src="../assets/story-img.jpg" alt="img-story" style="width: 30rem;">
        </div>
    </div>
</div>
<div class="bg-bottom reveal" style="position: relative;">
<div class="text-bottom" style="position: absolute;top: 50%;left: 50%;transform: translate(-50%,-50%);text-align: center;">
    <p class="title-bottom">Orderpickup</p>
    <h1 style="color: #fff;">Order Pickup & Delivery</h1>
    <button class="order">Order Pickup & Delivery</button>
    </div>
    
</div>
</template>

<script>
   export default {
    name: 'S-Story',
    data(){
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");

            for (var i = 0; i < reveals.length; i++) {
                var windowHeight = window.innerHeight;
                var elementTop = reveals[i].getBoundingClientRect().top;
                var elementVisible = 150;

                if (elementTop < windowHeight - elementVisible) {
                    reveals[i].classList.add("active");
                } else {
                    reveals[i].classList.remove("active");
                }
            }
}

window.addEventListener("scroll", reveal);
    }
   }
</script>

<style>

.reveal{
  position: relative;
  transform: translateY(150px);
  opacity: 0;
  transition: 1s all ease;
}

.reveal.active{
  transform: translateY(0);
  opacity: 1;
}

.c-story{
    width: 80%;
    height: 95vh;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.text-left,.img-right{
    flex: 1;
}
.text-left{
    position: relative;
}
.title-head{
    font-family: var(--font-snake);
    font-size: 7rem;
    color: var(--color-orange);
    text-shadow: 0 5px 10px rgba(0, 0, 0,0.3);

    position: absolute;
    top: 20%;
    left: 50%;
    transform: translate(-50%,-80%);
}

.title-bottom{
    font-family: var(--font-snake);
    font-size: 7rem;
    color: var(--color-orange);
    text-shadow: 0 5px 10px rgba(0, 0, 0,0.3);
}

h1{
    font-family: var(--font-text);
    font-size: 3rem;
    color: #262526;
    text-shadow: 0 5px 10px rgba(0, 0, 0,0.3);
}

h2{
    font-family: var(--font-text);
    font-size: 1rem;
    color: #424242;
}
span{
    font-family: var(--font-text);
    font-size: 1rem;
    color: #424242;
}
.about{
    font-size: 1.2rem;
    font-family: var(--font-text);
    color: var(--color-orange);
    transition: 300ms;
}
.about:hover{
    color: #262526;
}
.bg-bottom{
    width: 95%;
    height: 60vh;
    background-image: url(../assets/bg-img-2.jpg);
    background-size:cover;
    background-position: center;
    background-repeat: no-repeat;
    margin-left: auto;
    margin-right: auto;
    border-radius: 5px;
}
.order{
    padding: 5px 25px;
    border: 1px solid rgb(255, 8, 8);
    background: rgb(255, 8, 8);
    color: var(--text-color);
    font-family: var(--font-text);
    font-size: 16px;
    box-shadow: 0 5px 15px rgba(0, 0, 0,0.7);
    border-radius: 20px;
    cursor: pointer;
    transition: 300ms;
}
.order:hover{
    border: 1px solid var(--color-orange);
    background: rgb(35, 35, 35);
    color: var(--color-orange);
}

@media (max-width: 740px) {
    .c-story{
    flex-direction: column;
}
.title-head{
    position: absolute;
    top: 5%;
    left: 50%;
    transform: translate(-50%,-90%);
    font-size: 4rem;
}
.title-bottom{
    font-size: 4rem;
}
.bg-bottom{
    width: 100%;
}
}
</style>