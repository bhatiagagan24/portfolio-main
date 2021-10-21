<script>
let project_desc = 
[
    ["Url Shortener", "Project Description 1 line", "Tech Stack", "Github Url"],
    ["Url Shortener", "Project Description 1 line", "Tech Stack", "Github Url"],
    ["Url Shortener", "Project Description 1 line", "Tech Stack", "Github Url"],
    ["Url Shortener", "Project Description 1 line", "Tech Stack", "Github Url"],
    ["Url Shortener", "Project Description 1 line", "Tech Stack", "Github Url"],
];

var view_more_projects = 0;

</script>

<style>
hr {
    color: black;
}
</style>


<br>
<div class="flex flex-row align-middle justify-center text-center" style="color: black; background-color:blanchedalmond">
    <strong>Projects</strong>
</div>

<div class="py-2 md:py-4 grid gap-2 md:gap-4 grid-cols-1 md:grid-cols-3 lg:grid-cols-4 text-xl md:text-3xl text-center" style="margin-left: 1%; margin-right: 1%">
    {#each project_desc as project, i}
    <span class="flex flex-col project-card" style="color:black; border-color: black; border-width: 0.01em;">
        {#if view_more_projects === 0}
        {#if i < 4}
        <span class="text-lg md:text-2xl">{project[0]} </span>
        <span class="flex flex-col text-sm md:text-lg">
            <hr>
            <em>{project[1]} </em>
        </span>
        <span  style="color:black; margin-bottom:3%">
            <a href="https://github.com/bhatiagagan24">
                <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-github w-7 lg:w-10" viewBox="0 0 16 16" style="display:block; margin:auto; margin-top:2vh; margin-left: auto;">
                    <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
                  </svg>
            </a>
        </span>
        {:else if i >= 4}
        <span class="hidden md:flex flex-col">
            <span class="text-lg md:text-2xl">{project[0]} </span>
        <span class="flex flex-col text-sm md:text-lg">
            <hr>
            <em>{project[1]} </em>
        </span>
            <span  style="color:black; margin-bottom:3%">
                <a href="https://github.com/bhatiagagan24">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-github w-7 lg:w-10" viewBox="0 0 16 16" style="display:block; margin:auto; margin-top:2vh; margin-left: auto;">
                        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
                      </svg>
                </a>
            </span>
        </span>
        {/if}
        {:else}
        <span class="flex flex-col">
            <span class="text-lg md:text-2xl">{project[0]} </span>
        <span class="flex flex-col text-sm md:text-lg">
            <hr>
            <em>{project[1]} </em>
        </span>
            <span  style="color:black; margin-bottom:3%">
                <a href="https://github.com/bhatiagagan24">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-github w-7 lg:w-10" viewBox="0 0 16 16" style="display:block; margin:auto; margin-top:2vh; margin-left: auto;">
                        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
                      </svg>
                </a>
            </span>
        </span>
        {/if}
    </span>
    {/each}
</div>

{#if view_more_projects === 0}
<div class="sm:flex md:hidden flex-row align-middle justify-center text-center" style="color: black;"> 
    <button on:click={() => {view_more_projects = 1}} > View all skills </button>
</div>
{/if}
