<template>
    <div class="container" id="Home">
        <div class="bg-container">
            <div class="content">
                <h1 class="title-text">raksushi</h1>
                <h1 class="title">RAKSUSHI.</h1>
            </div>
            <button class="btn" id="#Home">EXPLORE</button>
        </div>
    </div>
</template>
    
<script>
export default {
    name: 'H-Home',
}
</script>
    
<style>


.container{
    width: 100%;
    height: 100vh;
}

.bg-container{
    height: 100%;
    background-image: url(../assets/bg-img-1.jpg);
    background-size:cover;
    background-position: center;
    background-repeat: no-repeat;
    position: relative;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.4);
}

.content{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);

    text-align: center;
}

.title-text{
    position: absolute;
    top: 10%;
    left: 50%;
    transform: translate(-50%,-60%);
    font-family: var(--font-snake);
    font-size: 10rem;
    color: var(--color-orange);
    text-shadow: 0 5px 15px rgba(0, 0, 0,0.8);
    animation: text-load 400ms ease-in;
}

.title{
    position: absolute;
    font-family: var(--font-text);
    font-size: 5rem;
    color: var(--text-color);
    text-shadow: 0 5px 15px rgba(0, 0, 0,0.8);
    animation: text-load 800ms ease-in;
}

.btn{
    margin-top: 10rem;
    padding: 5px 20px;
    border: 1px solid rgb(254, 132, 75);
    border-radius: 20px;
    font-family: var(--font-text);
    font-size: 14px;
    background: rgb(254, 132, 75);
    box-shadow: 0 5px 15px rgba(0, 0, 0,0.7);
    color: var(--text-color);
    cursor: pointer;
    transition: 200ms;
    animation: text-load 900ms ease-in-out;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}

.btn:hover{
    border: 1px solid var(--color-orange);
    background: rgb(35, 35, 35);
    color: var(--color-orange);
}

@keyframes text-load{
    0%{
        transform: scale(0)
    }
    90%{
        transform: scale(1.1)
    }
    100%{
        transform: translateX(1);
    }
}

@media (max-width: 740px) {
    .title-text{
    font-size: 5rem;
}

.title{
    font-size: 2rem;
}

}
</style>