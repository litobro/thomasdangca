<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>

<ModeWatcher />

<Header />

<main class="container max-w-6xl">
    <slot />
</main>

<Footer />