<script>
    import Footer from "../lib/Footer.svelte";

</script>
<div class="header">
    <h1>Rishabh Sambare</h1>
    <p>
        I'm a third-year student at the <a href="https://www.uwaterloo.ca">University of Waterloo</a> studying computer science. I'm currently a software engineer intern at Siemens,
        working on the <a href="https://www.enlightedinc.com/">Enlighted</a> research and architecture team.
        <br>
        <br>
        I previously spent time interning at <a href="https://tribalscale.com">TribalScale</a> developing serverless APIs with TypeScript and AWS for several projects. 
        Before that, I had a fantastic time interning on the <a href="https://distributedgenomics.ca">CanDIG team</a> at <a href="https://uhn.ca">UHN</a>, where I prototyped a federated learning system over their
        decentralized infrastructure for genomic data.
    </p>
    <Footer/>
</div>

<style>
    .header {
        flex: 1;
        display: flex;
        flex-flow: column nowrap;
        color: var(--header-text);
    }

    .header h1 {
        font-size: 30px;
        font-weight: normal
    }

    .header a {
        text-decoration: none;
        color: var(--link-body);
    }
</style>
