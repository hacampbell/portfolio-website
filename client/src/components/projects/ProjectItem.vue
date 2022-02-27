<template>
    <div class="project-item">
        <img v-bind:src="img">
        <h3>{{title}}</h3>
        <p>{{description}}</p>
        <button class="project-button" @click="OpenLive">LIVE</button>
        <button class="project-button" @click="OpenGitHub">GITHUB</button>
    </div>
</template>

<script>
    export default {
        name: 'ProjectItem',
        components: {},
        props: {
            title: String,
            description: String,
            img: String,
            live: String,
            github: String
        },
        methods: {
            OpenLive: function () {
                window.open(this.live, '_blank');
            },

            OpenGitHub: function () {
                window.open(this.github, '_blank');
            },
        }
    }
</script>

<style scoped>

    .project-item {
        background-color: #fff;
        margin: 5% 10%;
        max-width: 90%;
        color: #333;
        box-shadow: 0 0 2rem rgb(150 150 150 /120)
    }

    .project-item img {
        max-width: 100%;
        height: 25%;
    }

    .project-item h3 {
        margin-bottom: 1%;
        font-size: 200%;
    }

    .project-item p {
        margin: 5%;
    }

    .project-item button {
        padding: 2%;
        margin: 3%;
        background-color: #c83cb9;
        color: #fff;
        border: none;
        cursor: pointer;
        letter-spacing: 3px;
        width: 40%;
    }

    .project-item button:hover {
        font-weight: bold;
    }


</style>
