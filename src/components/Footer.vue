<template>
    <footer class="footer-container">
        <div class="footer">
            <div class="footer-contacts">
                <a name="contacts"></a>
                <p class="contact">Email: pokerniigenii12@gmail.com</p>
                <p class="contact">Number: 7(982) 498-43-42</p>
                <p class="contact">Github: <a href="https://github.com/rovonov98"></a>https://github.com/rovonov98</p>
            </div>
            <p>&copy; Copyright 2020</p>
        </div>
    </footer>
</template>

<style scoped lang="scss">
    .footer-container {
        background: $main-color-two;
        color: $main-color-one;
        padding: .5em;
        font-size: .8em;
        border-radius: 1%;
    }
    .footer {
        max-width: $main-container;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .footer-link {
        color: $main-color-one;
        text-decoration: none;
    }
    .contact {
        margin: .3em;
    }
</style>