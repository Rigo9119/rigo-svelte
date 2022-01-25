<script>
    import { jobs } from '../content/experience';
    import ExpCard from '../components/expCards.svelte'
</script>

<section class="experience">
    <h2 class="experience__title">
        I have worked for
    </h2>
    <div class="experience__cards">
        {#each jobs as job}
            <div class="job">
                <h3 class="job__title">{job.company}</h3>
                <div class="job__projects">
                    {#each job.projects as pr}
                        <ExpCard 
                            project={pr.project}
                            period={pr.period}
                            techs={pr.tech}
                            role={pr.role}
                            description={pr.description}
                        />
                    {/each}
                </div>
            </div>
        {/each}
    </div>

    <a class="back" href="/">
        Go back 
    </a>
</section>

<style lang="scss">
    .experience {
        display: flex;
        flex-flow: column nowrap;
        justify-content: space-around;
        margin: 45px 0;
        
        &__title {
            align-self: flex-start;
            //background: chartreuse;
            border-right: 22px solid chartreuse;
            color: white;
            font-size: 42px;
            margin: 0 auto;
            padding: 10px 30px;
            width: 88%;
        }

        &__cards {
            align-items: center;
            display: flex;
            flex-flow: column wrap;
            justify-content: space-around;
            width: 100%;

            .job {
                align-items: center;
                display: flex;
                flex-flow: column wrap;
                justify-content: space-around;
                margin: 35px 0;

                &__title {
                    color: chartreuse;
                    font-size: 26px;
                    padding: 22px;
                }

                &__projects {
                    align-items: center;
                    display: flex;
                    flex-flow: row wrap;
                    justify-content: space-around;
                    width: 100vw;
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
                background: chartreuse;
                border: 1px solid chartreuse;
                color: black; 
            }
        }
    }
</style>
