<script>
    import Icon from 'svelte-awesome';
    import { linkedin, github, at } from 'svelte-awesome/icons';    
</script>

<section class="contact"> 
    <h2 class="contact__title">
        Contact
    </h2>
    <div class="contact__btns">
        <a 
            class="contact__btns__btn" 
            href="https://www.linkedin.com/in/rigo-rosero97/"
            target="_blank">
            <Icon data={linkedin} scale="3" />
            <span class="contact__btns__btn__txt">
                Linkedin
            </span>
        </a>
        <a 
            class="contact__btns__btn" 
            href="https://github.com/Rigo9119"
            target="_blank">
            <Icon data={github} scale="3" />
            <span class="contact__btns__btn__txt">
                Github
            </span>
        </a>
        <a 
            class="contact__btns__btn" 
            href="mailto:rigo4791@gmail.com"
            target="_blank">
            <Icon data={at} scale="3" />
            <span class="contact__btns__btn__txt">
                Email
            </span>
        </a>
    </div>
    <a class="back" href="/">
        Go back 
    </a>
</section>

<style lang="scss">
    .contact {
        align-items: center;
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        height: 90vh;
        width: 100%;

        &__title {
            align-self: flex-start;
            //background: orange;
            border-right: 22px solid aqua;
            color: white;
            font-size: 42px;
            margin: 0 auto;
            padding: 10px 30px;
            width: 88%;
        }

        &__btns {
            align-items: center;
            display: flex;
            flex-flow: row nowrap;
            justify-content: space-between;
            width: 80%;
            &__btn {
                align-items: center;
                border: 1px solid white;
                border-radius: 5px;
                display: inline-flex;
                color: white;
                justify-content: space-between;
                padding: 10px 25px;
                text-decoration: none;
                width: 8%;

                &:hover {
                    width: 15%;
                    span {
                        display: block;
                    }
                }

                &__txt {
                    display: none;
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
                background: aqua;
                border: 1px solid aqua;
                color: black; 
            }
        }
    }
</style>
