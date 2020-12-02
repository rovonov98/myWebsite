<template>
    <section class="portfolio">
        <h2 class="portfolio-h2">My projects</h2>
        <div class="projects">
            <a name="portfolio"></a>
            <div class="project">
                <div class="portfolio-img"></div>
                <p>Something</p>
            </div>
            <div class="project">
                <div class="portfolio-img"></div>
                <p>Something2</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    
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
    }
    .portfolio-h2 {
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
    .portfolio-img {
        width: 10em;
        height: 10em;
        background-image: url('../assets/img/fishchips.jpg');
        background-size: cover;
        margin-bottom: .5em;
    }
</style>