<script lang="ts">
    import projects from './data/projects.json';
    import Card from './lib/Card.svelte';
</script>
<div class="projects">
    <h1>Projects</h1>
    <p>
        This is a collection of projects I've made (or am making). Several of these are old, small, or purely educational and probably shouldn't be used as a reference 
        of what 'good' software can look like.
    <br>
    <br>
        I enjoy producing software for my friends and the communities I'm involved in; I find it keeps the work meaningful.
    </p>
    <div class="project-card-list">
        {#each projects as project (project.id) }
            <Card {...project} />
        {/each}
    </div>
</div>
<style>
    .projects {
        flex: 1;
        display: flex;
        flex-flow: column nowrap;
        color: var(--header-text);
    }
    .projects h1 {
        font-size: 30px;
        font-weight: normal
    }
    .project-card-list {
        margin: auto;
    }
</style>