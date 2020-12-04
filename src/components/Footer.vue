<template>
    <footer class="footer-container">
        <div class="footer">
            <div class="footer-contacts">
                <a name="contacts"></a>
                <div class="contact">
                    <img class="img" src="../assets/img/gmail.svg" alt="">
                    <p>Mail:pokerniigenii12@gmail.com</p>
                </div>
                <div class="contact">
                    <img class="img" src="../assets/img/phone.svg" alt="">
                    <p>Number: 7(982) 498-43-42</p>
                </div>
                <div class="contact">
                    <img class="img" src="../assets/img/github.svg" alt="">
                    <p>Github: <a class="footer-link" href="https://github.com/rovonov98">https://github.com/rovonov98</a></p>
                </div>
                
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
        display: flex;
    }
    .img {
        max-width: 1em;
    }
</style>