<template>
    <div id="home">
        <Nav />
        <h3>— Hi there</h3>
        <h1>I'm Henry Campbell</h1>
        <h2>I study Computer Science</h2>
        <div class="gradient-overlay"></div>
    </div>
</template>

<script>
import Nav from '../components/Nav.vue'

export default {
  name: 'Home',
  components: {
    Nav
  }
}
</script>

<style scoped>
    h1 {
        font-size: 400%;
        text-align: left;
        padding-left: 35%;
        z-index: 1;
    }

    h2 {
        font-size: 300%;
        text-align: left;
        padding-left: 35%;
        z-index: 1;
    }

    h3 {
        color: #c83cb9;
        padding-top: 20%;
        font-size: 200%;
        text-align: left;
        padding-left: 30%;
        z-index: 1;
    }

    #home {
        background-color: rgb(17, 17, 17);
        height: 100vh;
        background-image: url(https://d33wubrfki0l68.cloudfront.net/images/f20315b799c67d762c3c2992f87aa674e6e30d19/hero-bg.jpg);
        background-repeat: no-repeat;
        background-size: 100% 100%;
        position: relative;
        z-index: 1;
    }

    .gradient-overlay {
        width: 100%;
        height: 100%;
        background: black;
        background-image: linear-gradient(to bottom, rgb(20, 20, 20), rgb(0, 0, 0));
        opacity: 0.95;
        position: absolute;
        left: 0;
        top: 0;
        z-index: -1;
    }
</style>
