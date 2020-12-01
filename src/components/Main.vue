<template>
    <section class="main">
        <h1 class="welcome">Hello, I'm Nikita</h1>
        <p class="description">A frontend developer</p>
        <a href=""></a>
    </section>
</template>

<style scoped lang="scss">
    .main {
        background-repeat: no-repeat;
        background-size: cover;
        min-height: 100vh;
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
            line-height: 2em;
            position: relative;
            
        }
    .description {
            font-size: 1.5em;
            position: relative;
    }
</style>