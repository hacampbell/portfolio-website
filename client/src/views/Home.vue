<template>
    <div id="content">
        <section id="home">
            <Splash />
        </section>

        <section id="about">
            <About />
        </section>

        <section id="projects">
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

<style>
    body {
        overflow: hidden;
    }


    #content {
        height: 100vh;
        overflow-y: scroll;
        scroll-behavior: smooth;
    }

    #home {
        min-height: 100vh;
    }

    #about {
        min-height: 100vh;
    }
</style>
