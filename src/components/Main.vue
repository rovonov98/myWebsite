<template>
    <section class="main">
        <h1 class="welcome">Hello, I'm Nikita</h1>
        <p class="description">A frontend developer</p>
        <a class="more" href="#about">More</a>
    </section>
</template>

<style scoped lang="scss">
    .main {
        background-repeat: no-repeat;
        background-size: cover;
        min-height: 105vh;
        max-width: 100%;
        color: $main-color-one;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        position: relative;
        margin: 0;
        background: radial-gradient(circle, rgba(2,0,36,1) 0%, rgba(0,0,0,1) 35%, rgba(30,144,255,1) 100%);
    }
    .welcome {
            font-size: 5em;
            position: relative;
            text-align: center;
        }
    .description {
            font-size: 1.5em;
            position: relative;
            line-height: 2em;
            margin-bottom: 1em;
    }
    .more {
        text-decoration: none;
        color: $main-color-two;
        padding: .8em 1.8em;
        border: 1px solid $main-color-two;
        font-size: 1.5em;
        font-weight: bold;
    }
</style>