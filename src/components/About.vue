<template>
    <section class="about-section">
        <div class="about">
            <div>
                <h2 class="about-h2">About me</h2>
            </div>
            <div class="about-description">
                <a name="about"></a>
                <!-- <div class="about-image"></div> -->
                <p class="description-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa harum molestias sint. Tempora officia reprehenderit autem aspernatur porro veritatis, minus voluptate dolorem commodi, consequuntur vero, sunt modi soluta nemo magnam?
                Ab commodi harum quia earum sint. Nam eum dicta temporibus ipsum corrupti, rerum esse? Sapiente delectus laudantium minus, repellat, veritatis praesentium assumenda consequuntur, debitis cum corporis sint illum. Soluta, debitis!
                Tempora, eius odio, accusamus similique suscipit consequatur recusandae enim cupiditate repellendus et expedita. Rem, magni sed nihil pariatur neque dolore earum, iusto ex quibusdam iste deleniti nobis tempore a non!
                Vero non unde molestias odio ipsam odit deleniti, distinctio voluptas rem quidem. Harum praesentium labore obcaecati fugit magnam sequi commodi id vero sit, omnis sunt quis unde culpa quos tempore!</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    .about-section {
        background: $main-color-two;
        padding: 1em;
        margin: 0;
        border-radius: 1%;
    }
    .about {
        display: flex;
        flex-direction: column;
        align-items: center;
        max-width: $main-container;
        color: $main-color-one;
        margin: 0 auto;
        .about-h2 {
            text-align: center;
            line-height: 2em;
            font-size: 3em;
        }
    }
    .about-description {
        line-height: 1.5em;
        display: flex;
        // justify-content: s;
        align-items: center;
    }
    .about-image {
        border-radius: 50%;
        background-image: url("../assets/img/questionMark.jpg");
        background-size: cover;
        width: 20em;
        height: 10em;
    }
    .description-text {
            margin: 1em;
            // max-width: 60%;
        }
</style>