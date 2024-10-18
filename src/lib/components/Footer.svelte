<script>
    export let session;

    const currentYear = new Date().getFullYear();
</script>

<footer class="flex flex-col items-center py-4 text-gray-600 mx-auto max-w-4xl">
    <div class="w-4/5 border-t border-gray-400"></div>
    <p class="text-center my-4">
        ©{currentYear} <a href="/contact" class="text-primary hover:text-orange-700">Thomas Dang</a>. 
        All rights reserved.
    </p>
    <div>
        Built using <a class="hover:text-orange-700" href="https://kit.svelte.dev/">SvelteKit</a>, <a class="hover:text-orange-700" href="https://www.shadcn-svelte.com/">shadcn-svelte</a>. 
        Hosted on <a class="hover:text-orange-700" href="https://pages.cloudflare.com/">Cloudflare Pages</a>.
    </div>
</footer>