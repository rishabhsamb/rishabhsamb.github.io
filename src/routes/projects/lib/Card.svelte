<script lang="ts">
    export let title: string;
    export let description: string;
    export let link: string;
</script>

<a class="project-card-link" href={link}>
    <div class="project-card">
        <div class="project-card-text">
        <h4><b>{title}</b></h4>
        <p>{description}</p>
        </div>
    </div>
</a>

<style>
    a, a:active, a:hover, a:visited {
        text-decoration: none;
        color: inherit;
    }
    .project-card {
        box-shadow: 0 2px 4px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        margin: 2em 0;
    }
    .project-card:hover {
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    }
    .project-card-text {
        padding: 0.25em 1em;
        display: inline-block;
    }
</style>