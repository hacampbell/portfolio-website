<template>
    <div id="about">
        <h2>ABOUT</h2>
        <h3>Personal Information</h3>
        <h4>Get to know more about me</h4>

        <div class="row">
            <!-- Left Column -->
            <div class="column">
                <h4>Hello!</h4>
                <p>
                    My name is Henry Campbell. I'm a Computer Science student at the University of New England majoring in Software Development in order to become a Software Engineer. I have particular interest in backend web development, data structures and algorithms, and desktop application development.
                </p>
                <p>
                    I’m currently looking to become part of a dedicated team of engineers responsible for building quality software, so if you’re hiring and like my sample work below, please feel free to contact me on LinkedIn. 
                </p>
                <p>
                    You can see some examples of my work below.
                </p>
            </div>

            <!-- Right Column -->
            <div class="column">
                <h4>Skills</h4>
                <ul id="skills">
                    <li>JavaScript</li>
                    <li>Node + Express</li>
                    <li>C/C++</li>
                    <li>Java</li>
                    <li>C#</li>
                    <li>Python</li>
                    <li>SQL</li>
                    <li>MongoDB</li>
                    <li>Git</li>
                    <li>Mac/Windows/Linux</li>
                </ul>
            </div>
        </div>

        <div id="scroll-down">
            <a href="#projects">View My Work</a>
            <br />
            <i class="fa fa-angle-down" style="font-size:20px"></i>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'About',
        components: {}
    }
</script>

<style scoped>
    h2 {
        color: #c83cb9;
        font-size: 175%;
        padding-top: 10rem;
        letter-spacing: 3px;
    }

    h3 {
        font-size: 200%;
        font-family: 'Libre Baskerville', serif;
        color: black;
        padding-top: 1rem;
    }

    h4 {
        font-size: 125%;
        color: black;
        padding-top: 1rem;
    }

    p {
        color: black;
        margin-top: 1rem;
        font-size: 110%;
        line-height: 1.5;
    }

    ul {
        margin-top: 1rem;
    }

    li {
        color: #333;
        list-style: none;
        font-size: 95%;
        margin: 0.5rem;
        background-color: #eee;
        display: inline-block;
        padding: 1% 4%;
    }

    li:hover {
        background-color: #c83cb9;
        color: #fff;
    }

    .row {
        display: flex;
        margin-left: 15rem;
        margin-right: 15rem;
    }

    .column {
        flex: 50%;
        margin: 5rem 1rem 5rem 1rem;
        text-align: left;
    }

    #about {
        background-color: rgb(255, 255, 255);
        height: 100%;
        text-align: center;
    }

    #scroll-down{
        margin: 5%;
        color: black;
    }

    #scroll-down a {
        text-decoration: none;
        color: black;
    }

    #scroll-down a:hover {
        font-weight: bold;
    }

    @media only screen and (max-width: 1150px) {
        h2 {
            padding-top: 5%;
        }

        h4 {
            padding-top: 1%;
        }

        .row {
           display: inline-block;
           margin-left: 10%;
           margin-right: 10%;
        }

        .column {
            margin: 8%;
        }
    }

</style>
