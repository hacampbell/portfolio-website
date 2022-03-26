<template>
    <div id="projects">
        <h2>PROJECTS</h2>
        <h3>Latest Work</h3>
        <h4>View a sample of my work here</h4>

        <div class="row">
            <div class="column">
                <ProjectItem
                    title="Drop Bear Table"
                    description="Drop Bear Table is a web application built using MongoDB, Express.js, Vue 3 and Node. Its purpose is to make table reservations at restaurants. I built this project to serve as a demonstration of my ability to work across the full web tech stack, and deal with features such as user authentication and authorisation."
                    live="https://github.com/hacampbell/table-reservations"
                    github="https://github.com/hacampbell/table-reservations"
                    img="dbt.png"
                />
            </div>

            <div class="column">
                <ProjectItem
                    title="Sudoku Solver"
                    description="A python implementation of depth first search to solve a 9x9 sudoku puzzle. Each position of the sudoku grid is iterated over, with a number valid by the game’s rules being placed in each position. In the case that a dead end is reached, the program back tracks and tries a new value in the previous position."
                    live="https://github.com/hacampbell/sudoku-solver-python"
                    github="https://github.com/hacampbell/sudoku-solver-python"
                    img="sudoku.png"
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
        padding-top: 2rem;
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

    @media only screen and (max-width: 1150px) {
        h2 {
            padding-top: 5%;
        }
    }

    @media only screen and (max-width: 1000px) {
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
