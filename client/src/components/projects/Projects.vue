<template>
    <div id="projects">
        <h2>PROJECTS</h2>
        <h3>Latest Work</h3>
        <h4>View a sample of my work here</h4>

        <div class="row">
            <div class="column">
                <ProjectItem
                    class="project-item"
                    title="Example Project 1"
                    description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum quo ipsum tenetur, magni numquam cupiditate quisquam harum perspiciatis delectus facilis! Labore sit soluta hic libero accusamus ipsa laboriosam laborum in."
                    live="https://google.com"
                    github="https://github.com/"
                    img="https://web.archive.org/web/20201226002509im_/https://d33wubrfki0l68.cloudfront.net/4343591e0826cbd40384e2841cf9851dec1d2017/9c7bb/images/gainon-mockup.jpg"
                />
            </div>

            <div class="column">
                <ProjectItem
                    class="project-item"
                    title="Example Project 2"
                    description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum quo ipsum tenetur, magni numquam cupiditate quisquam harum perspiciatis delectus facilis! Labore sit soluta hic libero accusamus ipsa laboriosam laborum in."
                    live="https://google.com"
                    github="https://github.com/"
                    img="https://web.archive.org/web/20201226002509im_/https://d33wubrfki0l68.cloudfront.net/4343591e0826cbd40384e2841cf9851dec1d2017/9c7bb/images/gainon-mockup.jpg"
                />
            </div>
        </div>

    </div>
</template>

<script>
    import ProjectItem from './ProjectItem.vue'

    export default {
        name: 'Projects',
        components: {
            ProjectItem
        }
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

    #projects {
        background-color: #e2e2e2;
        min-height: 100vh;
        text-align: center;
    }

    .row {
        display: flex;
    }

    .column {
        flex: 50%;
    }

    @media only screen and (max-width: 1000px) {
        h2 {
            padding-top: 5%;
        }

        .row {
           display: inline-block;
           margin-left: 10%;
           margin-right: 10%;
        }

        .column {
            margin: 1%;
        }
    }

</style>
