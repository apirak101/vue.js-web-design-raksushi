<template>
    <div class="c-menu reveal" id="Menu">
        <div class="img-menu-left reveal">
            <img src="../assets/prouct.jpg" alt="product" style="width: 30rem;">
        </div>
        <div class="text-menu-right">
            <p class="title-head-menu">menu</p>
            <h1>MENU</h1>
            <h2>✻</h2>
            <span>Fresh authentic sushi, professionally prepared. We create culinary works of art that are as delicious as
                they are beautiful. We proudly carry a large variety of the best sake and other refreshing adult beverages
                for your convenience and enjoyment.</span><br><br>
            <p><a href="#Menu" class="about">VIEW THE FULL MENU</a></p>
        </div>
    </div>
    <div class="bg-bottom-menu reveal" style="position: relative;">
        <div class="text-bottom" style="position: absolute;top: 50%;left: 50%;transform: translate(-50%,-50%);text-align: center;">
    <p class="title-bottom">Contact</p>
    <h1 style="color: #fff;">Contact</h1>
    <button class="Contact">Contact</button>
    </div>
    </div>
</template>

<script>
export default {
  name: 'M-Menu'
}
</script>

<style>
.c-menu{
    width: 80%;
    height: 100vh;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}
.img-menu-left,.text-menu-right{
    flex: 1;
}

.text-menu-right{
    position: relative;
}

.title-head-menu{
    font-family: var(--font-snake);
    font-size: 7rem;
    color: var(--color-orange);
    text-shadow: 0 5px 10px rgba(0, 0, 0,0.3);

    position: absolute;
    top: 20%;
    left: 50%;
    transform: translate(-50%,-80%);
}
.bg-bottom-menu{
    width: 95%;
    height: 60vh;
    background-image: url(../assets/bg-img-3.jpg);
    background-size:cover;
    background-position: center;
    background-repeat: no-repeat;
    margin-left: auto;
    margin-right: auto;
    border-radius: 5px;
    margin-bottom: 5rem;
}
.Contact{
    padding: 5px 35px;
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

.Contact:hover{
    border: 1px solid var(--color-orange);
    background: rgb(35, 35, 35);
    color: var(--color-orange);
}

@media (max-width: 740px) {
    .c-menu{
    flex-direction: column;
}
.title-head-menu{
    margin-top: 10px;
    position: absolute;
    top: 5%;
    left: 50%;
    transform: translate(-50%,-90%);
    font-size: 4rem;
}
.bg-bottom-menu{
    width: 100%;
  
}
}
</style>