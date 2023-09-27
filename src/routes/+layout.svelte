<script>
    import '../app.css';
    import Header from "../components/header.svelte";
</script>

<Header />

<slot />

<style lang="postcss">
    :global(html) {
        background-color: theme(colors.black);
        color: theme(colors.blue.100);
    }
</style>