<script>
    import { secondarySkills, skills, startingToLearn } from "../content/skils";
</script>

<section class="about">
    <h2 class="about__title">About me</h2>
    <p class="about__paragraph">
        I am a Front End Developer with almost four years of experience in
        Web Development. My skills are realeated to HTML, CSS and Javascript and 
        really interested in new technologies and blockchain is kind of a 
        new hobby and something that I really want to learn. 
    </p>
    <p class="about__paragraph">
        I have been working with agile methodolgies and really love working in a 
        team as i like to learn others because I believe that helps me to improve
        in a profesional and personal level. I am really pationate about what I do 
        and really enjoy creating and discovering new programming and tech stuff.
    </p>

    <p class="about__paragraph">
        Aside from Web Development im a huband and a father of a beatiful son, I lived and finish my bachelor in
        New Zealand and also I lived in South Korea (my wife is Korean), I love playing guitar, listen too music, 
        play video games and cooking. I am really interested in blockchain and Web3 and currently learning and reading 
        quite a lot about that.... is the trent dont judge :D. 
    </p>
</section>

<section class="skills">
    <h3 class="skills__title">
        Skills
    </h3>
    <div class="skills__lists">
        <div class="list">
            <h4 class="list__title">Main</h4>
            <ul class="list__wrapper">
                {#each skills as skill}
                    <li class="list__item">{skill}</li>
                {/each}
            </ul>
        </div>
    
        <div class="list">
            <h4 class="list__title">Secondary</h4>
            <ul class="list__wrapper">
                {#each secondarySkills as skill}
                    <li class="list__item">{skill}</li>
                {/each}
            </ul>
        </div>
    
        <div class="list">
            <h4 class="list__title">Learning</h4>
            <ul class="list__wrapper">
                {#each startingToLearn as skill}
                    <li class="list__item">{skill}</li>
                {/each}
            </ul>
        </div>
    </div>

    <a class="back" href="/">
        Go back 
    </a>
</section>

<style lang="scss">
    .about {
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        margin: 45px 0;

        &__title {
            align-self: flex-start;
            // animation: subtitle_bkg 1s linear;
            border-right: 22px solid orange;
            color: white;
            font-size: 42px;
            margin: 0 auto;
            margin-bottom: 40px;
            padding: 10px 30px;
            width: 88%;
        }

        &__paragraph {
            padding: 20px 180px;
        }
    }

    .skills {
        align-items: center;
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        margin: 45px 0;

        &__title {
            align-self: flex-start;
            border-right: 22px solid orange;
            color: white;
            font-size: 42px;
            margin: 0 auto;
            padding: 10px 30px;
            width: 88%;
        }

        &__lists {
            align-items: flex-start;
            display: flex;
            flex-flow: row wrap;
            justify-content: space-around;
            margin: 20px 0;
            width: 100%;
        }

        .list {
            &__title {
                font-size: 22px;
                margin: 20px;
            }
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
                background: orange;
                border: 1px solid orange;
                color: black; 
            }
        }
</style>
