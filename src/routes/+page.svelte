<svelte:head>
    <title>JarBottle's Card</title> 
</svelte:head>

<div class="w-full md:h-screen flex items-center justify-center p-3 md:px-0">
    <!-- <div class="bg-slate-300/60 w-full md:w-3/4 max-w-4xl rounded-3xl p-4 grid md:grid-cols-2 xl:grid-cols-3 gap-2">
        <div class="md:col-span-2 xl:col-span-3 border-b-2 border-b-slate-800 border-solid">
            <h1 class="font-bold text-4xl text-slate-800">JarBottle</h1>
        </div>
        <div class="flex justify-center md:justify-normal">
            <img src="/profile_picture.png" alt="" class="rounded max-h-64 max-w-64">
        </div>
        <div class="xl:col-span-2 w-full md:w-2/3 flex flex-wrap flex-col justify-center">
            <div class="grid gap-2">
                <ul class="grid gap-1">
                    <li>just your average chronically online person</li>
                    <li><span class="font-bold">Likes:</span> Videogames, Hardstyle and the subgenres, Coding, Comics</li>
                </ul>
                    <p>for me it currently is <Clock/></p>
                <div>
                    <Socials/>
                </div>

            </div>
        </div>
    </div> -->
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
