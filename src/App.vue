<template>
<div>
  <Header />
  <Home />
  <div class="story">
  <Ourstory />
  </div>
  <Menu />
  <Contact />
</div>

</template>

<script>
import Header from './components/Header.vue';
import Home from './components/Home.vue';
import Ourstory from './components/Ourstory.vue';
import Menu from './components/Menu.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    Header,
    Home,
    Ourstory,
    Menu,
    Contact,
  }
}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Arima+Madurai:wght@400;700;800&family=Island+Moments&family=Pinyon+Script&display=swap');
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

::-webkit-scrollbar{
  width: 15px;
}

::-webkit-scrollbar-track{
  background: #dddd;
}

::-webkit-scrollbar-thumb{
  background: #b15000;
}

html{
  scroll-behavior: smooth;
}

#app {
  --font-logo :'Island Moments', cursive;
  --font-text :'Arima Madurai', cursive;
  --font-snake :'Pinyon Script', cursive;
  --bg-color : rgba(18, 18, 18, 0.8);
  --text-color : #ffff;
  --color-orange : rgb(255, 159, 80);

}

.story{
  margin: 3rem 0;
}


</style>
