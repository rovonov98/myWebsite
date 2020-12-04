<template>
    <section class="portfolio">
        <h2 class="portfolio-h2">My projects</h2>
        <a name="portfolio"></a>
        <div class="projects">
            <div class="project" v-for="(pic, index) in pics" :key="index">
                <img  class="project-img" :src="getImgUrl(pic)" v-bind:alt="pic">
                <a class="project-description" :href="pic.link"><p class="project-name">{{ pic.text }}</p></a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            pics: [
                {
                image: 'form1.jpg',
                text: 'Application form',
                link: 'https://github.com/rovonov98/Reactive__Front-end__Test_'
                },
                {
                image: 'myWebsite2.jpg',
                text: 'My website',
                link: 'https://github.com/rovonov98/myWebsite'
                },
            ]
        }
    },
    methods: {
        getImgUrl(pic) {
        return require('../assets/img/portfolio/'+ pic.image )
        }
    }
}
</script>

<style scoped lang="scss">
    .portfolio {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        padding: 2em;
        background: #FFF;
    }
    .projects {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
    .portfolio-h2 {
        text-align: center;
        font-size: 3em;
        color: $main-color-two;
        opacity: .9;
        margin: 1em;
    }
    .project {
        display: flex;
        flex-direction: column;
        margin: 1em;
        text-align: center;
        border: 1px solid #aaa;
        box-shadow: 0 .2em .2em #aaa;
        padding: .5em;
    }
    .project-img {
        max-width: 20vw;
    }
    .project-description {
        padding: 1em;
        text-decoration: none;
        color: $main-color-two;
        font-size: 1.5em;
    }
    @media(max-width: 992px) {
        .project-img {
            max-width: 35vw;
        }
    }
    @media(max-width: 768px) {
        .project-img {
            max-width: 40vw;
        }
    }
    @media(max-width: 576px) {
        .project-img {
            max-width: 80vw;
        }
    }
</style>