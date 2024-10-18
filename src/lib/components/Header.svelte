<script>
    import { title } from "$lib/config.js";

    import Sun from "lucide-svelte/icons/sun";
    import Moon from "lucide-svelte/icons/moon";
    import { toggleMode } from "mode-watcher";
</script>

<nav class="bg-accent px-4 border-b border-secondary mb-2">
    <div class="container max-w-6xl mx-auto py-1 sm:py-2 flex flex-wrap items-center justify-center sm:justify-between">
        <a href="/" class="flex items-center justify-center sm:justify-start space-x-3">
            <span class="self-center text-3xl text-primary font-semibold whitespace-nowrap">{title}</span>
        </a>
        <div class="w-full sm:w-auto mt-1 sm:mt-0">
            <ul class="font-medium flex flex-wrap justify-center sm:justify-end p-0 rounded-lg space-x-4 sm:space-x-8">
                {#each [
                    { href: "/", label: "Home" },
                    { href: "/about", label: "About" },
                    { href: "/cv", label: "CV" },
                    { href: "/nerd", label: "Nerd stuff" },
                    { href: "/contact", label: "Contact" },
                ] as item}
                <li>
                    <a href={item.href} class="block py-1 sm:py-2 px-3 text-foreground hover:text-primary">{item.label}</a>
                </li>
                {/each}
                <li>
                    <button on:click={toggleMode} variant="outline" size="icon" class="flex m-2">
                        <Sun class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0" />
                        <Moon class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100" />
                        <span class="sr-only">Toggle theme</span>
                    </button>
                </li>
            </ul>
        </div>
    </div>
</nav>