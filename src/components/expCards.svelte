<script>
    export let project, period, role, description, techs;
</script>

<div class="project">
    <h4 class="project__title">{project}</h4>
    <h5 class="project__period">{period}</h5>
    <h6 class="project__role">{role}</h6>
    <p class="project__desc">{description}</p>
    <p class="project_subTitle">techs:</p>
    <ul class="project__techs">
        {#each techs as tech}
            <li class="project__tech">{tech}</li>
        {/each}
    </ul>
</div>

<style lang="scss">
    .project {
        width: 280px;

        &__title {
            padding: 6px;
        }
        &__period {
            padding: 6px;
        }
        &__role {
            padding: 6px;
        }
        &__desc {
            padding: 6px;
        }
        &__subtitle {
            padding: 6px;
        }
        &__techs {
            padding: 6px;

            &__tech {}
        }
    }
</style>
