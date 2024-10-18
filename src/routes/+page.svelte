<style>
    .text-shadow {
        text-shadow: 4px 4px 8px black; /* Enhanced shadow for better readability */
    }
    .overlay {
        background-color: rgba(0, 0, 0, 0.3); /* Dark overlay with 50% opacity */
    }
</style>

<div class="min-h-[80vh] flex flex-col">
    <div class="min-h-[60vh] h-full relative flex flex-col justify-center items-center bg-cover bg-center border border-secondary" 
        style="background-image: url('/assets/images/20240816_181621.jpg');">
        
        <!-- Background overlay -->
        <div class="overlay absolute inset-0"></div>

        <!-- Text content with shadow applied -->
        <div class="relative text-center text-white">
            <h1 class="text-shadow text-4xl font-semibold mb-4">Hi! I'm Thomas.</h1>
            <div class="mx-auto w-3/4 border-t border-white"></div>
            <div class="text-shadow text-xl">I'm an Information Security Professional, and a recovering politician.</div>
        </div>
    </div>

    <div class="flex-grow flex items-center justify-center">
        <div class="m-4 text-center font-semibold">
            Yukon Territorial Government Systems Architect (Cybersecurity), software consultant, hiker, cat-dad, runner, ADHD hyper-fixator. 
            <br />
            Still trying to make the world a better place.
        </div>
    </div>
</div>
