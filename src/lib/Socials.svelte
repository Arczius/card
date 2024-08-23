<ul class="flex flex-wrap gap-2">
    {#each socials as social}
        <li class="w-full grid">
            <a href="{social.link}" target="_blank" class="flex p-2 bg-slate-200 rounded-xl justify-center text-neutral-800 hover:bg-slate-300 focus:bg-slate-300">
                <div class="grid grid-cols-3 max-w-32">
                    <div class="col-span-1/1"><Icon icon="{social.icon}" color="{social.colour}" height="{social.size}" width="{social.size}"/></div>
                    <div class="col-span-2/3">{social.name}</div>
                </div>
            </a>
        </li>
    {/each}
</ul>

<script>
    import Icon from '@iconify/svelte';

    const socials = [
        {
            icon: "mdi:spotify",
            size: "28",
            colour: "#1DB954",
            link: "https://open.spotify.com/user/3123lrnctw5kvuxtomksnpokrnbu?si=aa5c74ca481c4787",
            name: "Spotify"
        },
        {
            icon: "mdi:steam",
            size: "28",
            colour: "#1b2838",
            link: "https://steamcommunity.com/id/jarbottle",
            name: "Steam"
        },
        {
            icon: "mdi:github",
            size: "28",
            colour: "#171515",
            link: "https://github.com/Arczius",
            name: "GitHub"
        },
        {
            icon: "mdi:lastfm",
            size: "28",
            colour: "#D51007",
            link: "https://www.last.fm/user/JarBottle",
            name: "Last.fm"
        },
        {
            icon: "clarity:cd-dvd-solid",
            size: "28",
            colour: "#000",
            link: "https://www.discogs.com/user/jarbottle/collection",
            name: "Discogs"
        },
        {
            icon: "simple-icons:trakt",
            size: "26",
            colour: "#ED1C24",
            link: "https://trakt.tv/users/jarbottle",
            name: "Trakt.tv"
        },
        {
            icon: "simple-icons:myanimelist",
            size: "26",
            colour: "#2e51a2",
            link: "https://myanimelist.net/profile/JarTheBottle",
            name: "MyAnimeList"
        },
    ]
</script>

