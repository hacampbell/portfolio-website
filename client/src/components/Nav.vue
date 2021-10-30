<template>
    <div id="nav">
        <router-link to="/">HOME</router-link>
        <router-link to="/about">ABOUT</router-link>
        <router-link to="/projects">PROJECTS</router-link>
    </div>
</template>

<script>
    export default {
    name: 'Nav',
    }
</script>

<style scoped>
    #nav {
        text-align: left;
        padding-left: 2rem;
        padding-top: 2rem;
    }

    a {
        font-weight: bold;
        margin-right: 3rem;
        color: white;
        text-decoration: none;

    }

    a.router-link-active, a:hover {
        border-bottom: 2px solid #96179b;
    }
</style>
