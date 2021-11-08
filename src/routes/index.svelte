<script>

import Social from "../components/social.svelte";
import Skills from "../components/skillscroll.svelte";
import Projects from "../components/projects.svelte";

let nameColor = "purple";



function changeColor() {
    if(nameColor === "green") {
    nameColor = "purple";
    } else {
        nameColor = "green";
    }
}

// $: setInterval(changeColor, 1500);


</script>

<svelte:head>
    <title>Portfolio</title>
</svelte:head>

<style>

</style>

<main>
   
<br>
<!-- flexbox-centered
items-center -->
<div class="pt-10 uppercase align-middle text-md lg:text-2xl md:text-3xl flex  flex-col justify-center text-left divone sm:margin-top=0vh">
    <span class=" pl-5 flex flex-col flexbox-centered"> Hey, I am </span> 
    <strong><span style="color: {nameColor}" class=" pl-5 text-lg lg:text-3xl items-center"> Gagandeep <span> Bhatia </span></span></strong>
    
    <p class=" text-sm lg:text-2xl">
        <br>
    <i class="pl-5">Always Learning | Software Developer</i>
    </p>

    <!-- <div class=" flex flexbox-centered items-center flex-row justify-center text-center align-middle text-xl divone">
        <span class = "animate-bounce" > This is my Portfolio </span>
     </div> -->
     <br>
     
</div>

<!-- <div class="py-4 grid gap-4 md:grid-cols-2 grid-cols-1 text-xl md:text-3xl" >
    <span class="rounded-md hover:shadow-md flex flex-col items-center cardclass">
        <div>
            <p class="text-center" style="background-color:black; color:white">
                Education
            </p>
            <p>
                Description of my education here
            </p>
        </div>
    </span>
    <span class="rounded-md hover:shadow-md flex flex-col items-center">
        Education
    </span>        
</div> -->


<div>
    <Social />
</div>
<br>
<div>
    <Skills />
</div>
<div>
    <Projects />
    
</div>
<p></p>
</main>
