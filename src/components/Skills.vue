<template>
    <section class="skills-outer">
        <div class="skills-section">
            <a name="skills"></a>
            <h2 class="skills-h2">My skills</h2>
            <div class="skills-container">
                <ul class="skills">
                    <li class="skills-li" v-for="(skill, index) in skills" :key="index">{{ skill }} </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>

export default {
    data() {
        return {
            skills: ['HTML', 'CSS', 'JavaScript', 'Bootstrap', 'SCSS', 'GSAP', 'Vue', 'Vuex', 'Nuxt', 'gulp', 'jQuery']
        }
    }
}
</script>

<style scoped lang="scss">
    .skills-outer {
        background-color: #FFF;
    }
    .skills-section {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: 0 auto;
        padding: 1em 0 5em 0;
        max-width: $main-container;
    }
    .skills-h2 {
        text-align: center;
        font-size: 3em;
        margin: 2em;
        color: $main-color-two;
        opacity: .9;
    }
    .skills {
        display: flex;
        flex-wrap: wrap;
        max-width: 100%;
    }
    .skills-li {
            font-size: 1.3em;
            text-align: center;
            list-style: none;
            margin: 1em;
            background: $main-color-two;
            color: $main-color-one;
            padding: 1em;
            border-radius: 10%;
            user-select: none;  
            cursor: pointer;
        }
</style>