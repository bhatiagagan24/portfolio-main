<script>
    
   const skill_list = ["Python", "JavaScript", "Flask", "Svelte", "Flutter", "C++", "MySQL", "SQLite", "Azure", "AWS", "HTML"];

   var skill_to_be_displayed = ["Python", "JavaScript", "Flask", "Svelte", "Flutter"];

    // left rotate the list every 2-3 seconds
    function skill_selector() {

        for(var i = 0; i < skill_list.length - 1; i++) {
            var temp_var = skill_list[i];
            skill_list[i] = skill_list[i+1]; 
            skill_list[i+1] = temp_var;
        }
        skill_to_be_displayed = [];
        for(var i = 0; i<5; i++) {
            skill_to_be_displayed.push(skill_list[i]);
        }
        // skill_to_be_displayed = skill_list.splice(0, 5);
    }

    // $: setInterval(skill_selector, 5000);

    // button to display more skills pressed only if the value of this var is 0
    var more_skills_button_clicked = 0;

</script>

<style>
    button {
        color: white;
        border-width: 1.5vh;
        background-color: black;
        border-color: black;
    }
</style>

<div class="flex flex-row align-middle justify-center text-center" style="color: black; background-color:#DBFFFC">
    <strong>Skills</strong>
</div>


<div class="py-2 md:py-4 grid gap-2 md:gap-4 grid-cols-2 md:grid-cols-3 lg:grid-cols-4 text-md md:text-xl text-center ">
{#each skill_list as skill, i}
<span class="flex flex-col" style="color: black; backround-color: azure; margin-left:1em; margin-right: 1em">
    {#if more_skills_button_clicked === 0}
    {#if i < 4}
    <span class="border-4 hover:bg-gray-400 hover:text-white">
        <!-- <span class="hover:text-white"> -->
    {skill_list[i]}
<!-- </span> -->
    </span>
    {:else if i >= 4}
    <span class="hidden md:flex flex-col border-4 hover:bg-gray-400 hover:text-white">
        {skill_list[i]}
    </span>
    {/if}
    {:else}
    <span class="flex flex-col border-4 hover:bg-gray-400 hover:text-white">
        {skill_list[i]}
    </span>
    {/if}
</span>

{/each}

</div>
{#if more_skills_button_clicked === 0}
<div class="sm:flex md:hidden flex-row align-middle justify-center text-center" style="color: black;"> 
    <button on:click={() => {more_skills_button_clicked = 1}} > View all skills </button>
</div>
{/if}

