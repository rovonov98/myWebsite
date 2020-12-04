<template>
    <header class="header">
        <nav class="nav">
            <div class="logo nav-link">
                <a class="nav-a" href="#home">HOME</a>
            </div>
            <ul class="navbar">
                <li class="nav-link"><a class="nav-a" href="#skills">SKILLS</a></li>
                <li class="nav-link"><a class="nav-a" href="#about">ABOUT</a></li>
                <li class="nav-link"><a class="nav-a" href="#portfolio">PORTFOLIO</a></li>
                <li class="nav-link"><a class="nav-a" href="#contacts">CONTACS</a></li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
    .header{
        position: sticky;
        z-index: 2;       
        max-width: 100%; 
        top: 0;
        left: 0;
        right: 0;
        margin-left: auto;
        margin-right: auto;
        background: $main-color-two;
        border-radius: 1%;
    }
    .nav {
        margin: 0 auto;
        max-width: $main-container;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .navbar {
        display: flex;
        list-style: none;
        justify-content: space-between;
        max-width: 100%;
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
    }
</style>