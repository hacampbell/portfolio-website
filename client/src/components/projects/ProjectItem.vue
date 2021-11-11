<template>
    <div class="project-item">
        <!-- <img src="https://web.archive.org/web/20201226002509im_/https://d33wubrfki0l68.cloudfront.net/4343591e0826cbd40384e2841cf9851dec1d2017/9c7bb/images/gainon-mockup.jpg"> -->
        <img v-bind:src="img">
        <h3>{{title}}</h3>
        <p>{{description}}</p>
        <button class="project-button">LIVE</button>
        <button class="project-button">GITHUB</button>
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
