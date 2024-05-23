<h3 class="font-bold">Socials:</h3>
<ul class="flex gap-2">
    {#each socials as social}
        <li>
            <a href="{social.link}" target="_blank">
                <Icon icon="{social.icon}" color="{social.colour}" height="{social.size}" width="{social.size}"/>
            </a>
        </li>
	{/each}
</ul>

<script>
    import Icon from '@iconify/svelte';

    let socials = [
        {
            icon: "mdi:spotify",
            size: "28",
            colour: "#1DB954",
            link: "https://open.spotify.com/user/3123lrnctw5kvuxtomksnpokrnbu?si=aa5c74ca481c4787"
        },
        {
            icon: "mdi:steam",
            size: "28",
            colour: "#1b2838",
            link: "https://steamcommunity.com/id/jarbottle",
        },
        {
            icon: "mdi:github",
            size: "28",
            colour: "#171515",
            link: "https://github.com/Arczius",
        },
        {
            icon: "mdi:lastfm",
            size: "28",
            colour: "#D51007",
            link: "https://www.last.fm/user/JarBottle",
        },
    ]
</script>

