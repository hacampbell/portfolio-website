<template>
    <div id="content">
        <section id="home">
            <Splash />
        </section>

        <section id="About">
            <About />
        </section>

        <section id="Projects">
            <Projects />
        </section>
    </div>
</template>

<script>
    import Splash from '../components/splash/Splash.vue';
    import About from '../components/about/About.vue';
    import Projects from '../components/projects/Projects.vue'

    export default {
        name: 'Home',
        components: {
            Splash,
            About,
            Projects
        }
    }

</script>

<style scoped>

    /* #content {
        height: 100vh;
    } */

    section {
        height: 100vh;
    }
</style>
