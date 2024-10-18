<script>
    import Sun from "lucide-svelte/icons/sun";
    import Moon from "lucide-svelte/icons/moon";
    import { toggleMode } from "mode-watcher";
</script>

<h1 class="text-2xl font-bold m-2">Welcome to SvelteKit</h1>
<p class="m-2">Visit <a class="text-blue-500 hover:text-blue-600 hover:underline" href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button on:click={toggleMode} variant="outline" size="icon" class="flex m-2">
    <Sun class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0" />
    <Moon class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100" />
    <span class="sr-only">Toggle theme</span>
</button>