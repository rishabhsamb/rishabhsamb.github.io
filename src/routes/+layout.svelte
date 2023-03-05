<script lang="ts">
    import Navbar from "../lib/Navbar.svelte";
    import Footer from '../lib/Footer.svelte';
    import './globals.css';
</script>

<div class="container">
    <Navbar/>
    <slot/>
</div>

<style>
    .container {
        flex: 1;
        display: flex;
        flex-flow: column;
        margin: 50px auto;
        max-width: 750px;
        width: 100%;
    }
</style>
