<svelte:head>
    <title>JarBottle's Card</title> 
</svelte:head>

<div class="w-full md:h-screen flex items-center justify-center p-3 md:px-0">
    <div class="bg-neutral-800/90 w-full md:w-3/4 max-w-4xl p-4 rounded-3xl grid md:grid-cols-2 xl:grid-cols-3 gap-4">
        <div>
            <div class="flex gap-2 items-center w-full">
                <img src="/profile_picture.png" alt="" class="rounded-full max-h-16 max-w-16">
                <h2 class="font-bold text-4xl text-slate-200">JarBottle</h2>
            </div>
            <div class="text-slate-200 p-1">
                <p>Just your average chronically online person</p>
                <p>
                    <b>Likes:</b>
                </p>
                <ul class="list-disc pl-4">
                    <li>Music</li>
                    <li>Videogames</li>
                    <li>Coding</li>
                    <li>Comics</li>
                    <li>Anime/Manga</li>
                    <li>Movies</li>
                </ul>
                <br>
                <p>For me it currently is: <span class="text-green-400"><Clock/></span></p>
            </div>
        </div>
        <div class="xl:col-span-2 w-full flex flex-wrap flex-col justify-center">
            <h3 class="md:hidden text-slate-200 font-bold text-xl pb-1">Socials:</h3>
            <Socials/>
        </div>
    </div>
</div>

<script>
    import Clock from "$lib/Clock.svelte";
    import Socials from "$lib/Socials.svelte";
</script>
