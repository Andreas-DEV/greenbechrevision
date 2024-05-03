<script lang="ts">
    import "../app.css";
    import Navbar from "$lib/Navbar.svelte";
    import introVid from "$lib/assets/introvideo.mp4";
</script>

<Navbar />
<section class="dark:bg-gray-900 my-20 container mx-auto">
    <div
        class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12"
    >
        <div class="mr-auto place-self-center lg:col-span-7">
            <h1
                class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white"
            >
                Bogføring behøver ikke at være svært
            </h1>
            <p
                class="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400"
            >
                Velkommen til vores virksomhed, hvor vi tilbyder en bred vifte
                af services inden for bogføring og regnskab, kodning og
                webhosting. Vores dedikerede medarbejdere står klar til at
                hjælpe dig med dine forretningsbehov og sikre, at du får den
                bedst mulige support.
            </p>
            <a
                href="#"
                class="inline-flex items-center justify-center px-5 py-3 mr-3 text-base font-medium text-center text-white rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900"
            >
                Kom i gang
                <svg
                    class="w-5 h-5 ml-2 -mr-1"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                    ><path
                        fill-rule="evenodd"
                        d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                        clip-rule="evenodd"
                    ></path></svg
                >
            </a>
            <a
                href="https://dk.trustpilot.com/review/www.officeboost.dk" target="_blank"
                class="inline-flex items-center justify-center px-5 py-3 text-base font-medium text-center text-gray-900 border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800"
            >
                Udforsk reviews
            </a>
        </div>
        <div class="hidden lg:mt-0 lg:col-span-5 lg:flex gap-2">
            <div class="flex flex-col gap-4">
                <!-- svelte-ignore a11y-media-has-caption -->
                <video controls class="rounded h-[750px]" src={introVid} />
                <p class="text-center whitespace-nowrap leading-3"><span class="font-bold text-gray-800">Berith Nanett Grønbech</span><br><span class="italic text-sm">Indehaver/Bogholder</span></p>
            </div>
        </div>
    </div>
</section>
