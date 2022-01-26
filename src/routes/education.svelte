<section class="education">
    <h2 class="education__title">
        Education
    </h2>
    <p class="education__paragraph">
        Well im a self thaught developer, actually I have a Bachelor of Recording Arts but live had 
        a different plan for me, I still enjoy making and recording music but technology is a big part 
        of my life so being part of such an interesting industry has allow me to thrive in ways that probably 
        i wouldnt find in the music industry. Also im a father now and being close to my family is a priority :).
    </p>
    <p class="education__paragraph--center">
        So without keep extending this is my "normal" education
    </p>
    <ul class="education__list">
        <li class="education__list__item">
            Bogota Dev - Bootcamp
        </li>
        <li class="education__list__item">
            SAE Institute - Bachelor of Recording Arts
        </li>
    </ul>
    <p class="education__paragraph">
        Apart from that I have studied with different web plattaforms such as Udemy and Pluralsight but deffinetly
        the one that has help me the most is Front end Masters :D. 
    </p>
    <a class="back" href="/">
        Go back 
    </a>
</section>

<style lang="scss">
    .education {
        align-items: center;
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        height: 100vh;
        margin: 45px 0;

        &__title {
            align-self: flex-start;
            //background: orange;
            border-right: 22px solid blueviolet;
            color: white;
            font-size: 42px;
            margin: 0 auto;
            padding: 10px 30px;
            width: 88%;
        }

        &__paragraph {
            width: 83%;

            &--center {
                align-self: center;
            }
        }

        &__list {
            align-items: center;
            display: flex;
            flex-flow: column wrap;
            justify-content: space-around;
            margin: 20px 0;
            width: 100%;

            &__item {
                margin-bottom: 20px;
            }
        }

        .back {
            align-self: center;
            border: 1px solid white;
            border-radius: 2px;
            color: white;
            padding: 10px 22px; 
            text-decoration: none;

            &:hover {
                background: blueviolet;
                border: 1px solid blueviolet;
                color: black; 
            }
        }
    }
</style>
