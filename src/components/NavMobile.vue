<template>
    <div class="header-mobile">
        <a name="home"></a>
        <nav class="nav">
            <ul class="navbar">
                <li class="nav-link"><a class="nav-a" href="#home">HOME</a></li>
                <li class="nav-link"><a class="nav-a" href="#skills">SKILLS</a></li>
                <li class="nav-link"><a class="nav-a" href="#portfolio">PORTFOLIO</a></li>
            </ul>
        </nav>
    </div>
</template>

<style scoped lang="scss">
    .header-mobile{
        display: none;
        position: fixed;
        max-width: 100%; 
        top: 0;
        left: 0;
        background: $main-color-two;
        border-radius: 1%;
    }
    .nav {
        display: flex;
    }
    .navbar {
        display: flex;
        list-style: none;
        position: absolute;
        left: 0;
        height: 100vh;
        top: 0;
        background: $main-color-two;
        display: flex;
        flex-direction: column;
        width: 50vw;
        text-align: center;
        font-size: 1.5em;
        font-weight: bold;
        justify-content: center;
    }
    .nav-link {
        :hover {
            background:	$main-color-hover;
        }
        :active {
            background:$main-color-active;
        }
    }
    .nav-a {
        text-decoration: none;
        color: $main-color-one;
        display: block;
        max-width: 100%;
        padding: 1.5em;
        letter-spacing: .1em
    }
    @media(max-width: 768px) {
        .header-mobile {
            display: block;
        }
    }
</style>