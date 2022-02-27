<template>
    <div id="home">
        <Nav />
        <h3>— Hi there</h3>
        <h1>I'm Henry Campbell</h1>
        <h2>I study Computer Science</h2>
        <div class="gradient-overlay"></div>

        <svg id="gitsvg" xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24">
            <path id="github" @click="OpenGitHub" d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
        </svg>

        <svg id="linkedsvg" xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24">
            <path id="linkedin" @click="OpenLinkedIn" d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
        </svg>

        <div id="scroll-down">
            <a href="#about">Scroll Down</a>
            <br />
            <i class="fa fa-angle-down" style="font-size:20px"></i>
        </div>
    </div>
</template>

<script>
    import Nav from '../generic/Nav.vue'

    export default {
        name: 'Splash',

        components: {
            Nav
        },

        methods: {
            OpenLinkedIn: function () {
                window.open('https://au.linkedin.com','_blank');
            },

            OpenGitHub: function () {
                window.open('https://github.com/hacampbell','_blank');
            }
        }

    }
</script>

<style scoped>
    h1 {
        font-size: 400%;
        text-align: center;
        font-family: 'Libre Baskerville', serif;
        z-index: 1;
    }

    h2 {
        font-size: 300%;
        font-family: 'Libre Baskerville', serif;
        text-align: center;
        z-index: 1;
    }

    h3 {
        color: #c83cb9;
        margin-top: 20%;
        margin-right: 35%;
        font-size: 200%;
        text-align: center;
        z-index: 1;
    }

    svg {
        padding-top: 3rem;
    }

    #linkedsvg {
        padding-left: 3rem;
    }

    svg path {
        fill: white;
        margin-right: 10px;
    }

    svg path:hover {
        fill: #c83cb9;
        cursor: pointer;
    }

    #home {
        background-color: rgb(17, 17, 17);
        height: 100%;
        background-image: url('~@/assets/img/mountain2.jpg');
        background-repeat: no-repeat;
        background-size: 100% 100%;
        position: relative;
        z-index: 1;
    }
    
    #scroll-down{
        margin: 5%;
    }

    #scroll-down a {
        color: white;
        text-decoration: none;
    }

    #scroll-down a:hover {
        font-weight: bold;
    }

    .gradient-overlay {
        width: 100%;
        height: 100%;
        background: black;
        background-image: linear-gradient(to bottom, rgb(20, 20, 20), rgb(0, 0, 0));
        opacity: 0.70;
        position: absolute;
        left: 0;
        top: 0;
        z-index: -1;
    }

    @media screen and (max-width: 992px) {
        h1 {
            font-size: 300%;
            margin-top: 2%;
        }

        h2 {
            font-size: 200%;
            margin-top: 5%;
        }

        h3 {
            font-size: 175%;
            margin-top: 50%;
        }

        #home {
            overflow-x: hidden;
        }

        #scroll-down {
            margin-top: 20%;
        }

    }
</style>
