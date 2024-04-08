<script lang="ts">
    import mode from "$lib/mode.svg";
    import violet from "$lib/violet.svg";
    import sport from "$lib/sport.svg";
    import saintv from "$lib/saintv.svg";
    import app from "$lib/app.svg";
    import davix from "$lib/davix.svg";
    import kenneth from "$lib/kenneth.svg";
    import moon from "$lib/moon.svg";

    interface Website {
        src: string;
        alt: string;
        href: string;
    }

    let name: Website[] = [
        { src: mode, alt: "Logo Mode", href: "https://mode.com" },
        { src: violet, alt: "Logo Violet", href: "https://violet.com" },
        { src: sport, alt: "Logo Sport", href: "https://sport.com" }
    ];

    let figma: Website[] = [
        { src: mode, alt: "Figma Mode", href: "https://mode.com" },
        { src: saintv, alt: "Figma Saintv", href: "https://violet.com" },
        { src: app, alt: "Figma App", href: "https://sport.com" }
    ];

    let logo: Website[] = [
        { src: davix, alt: "Logo Davix", href: "https://mode.com" },
        { src: kenneth, alt: "Logo Kenneth", href: "https://violet.com" },
        { src: moon, alt: "Logo Moon", href: "https://sport.com" }
    ];
</script>




<main >

    <div class="trait" role="presentation" aria-hidden="true"></div>
<h3>
    My Projects ux&ui <br>
website,logo,and  <br>
figma design  <br>
</h3>


<h4>
    website
</h4>

<p>
    Create with svelte sveltekit <br>
database supabase and drizzle <br>
my start up or team project its private <br>
i would like show you that <br>
  
</p>

<div class="website">
    {#each name as {src , alt , href} }
       
    <a {href}>
        <img {src} {alt}  />
    </a>
    
   
    {/each}
</div>

<h4 class="autre">
design website figma
</h4>

<p class="autre">
    Create with svelte sveltekit <br>
database supabase and drizzle <br>
my start up or team project its private <br>
i would like show you that <br>
  
</p>
<div class="website">
    {#each figma as {src , alt , href} }
       
    <a {href}>
        <img {src} {alt}  />
    </a>
    
   
    {/each}
</div>




<h4 >
    logo 
</h4>

<p>
    Create with svelte sveltekit <br>
database supabase and drizzle <br>
my start up or team project its private <br>
i would like show you that <br>
  
</p>

<div class="website">
    {#each logo as {src , alt , href} }
       
    <a {href}>
        <img {src} {alt}  />
    </a>
    
   
    {/each}
</div>



<h3>
    definitly thank for <br>
    taking your time for <br>
    wath my potfolio take <br>
    care and keep going <br>
    to create  <br>
</h3>


</main>



<style lang="scss">
  @use "$lib/variable" as *;
main{
     margin-top: 80px;
      
h3{
    margin-left: 15%;
    font-size: 4em;
    font-family: $font, sans-serif;
  
}
h4{
    margin-left: 70%;
    font-size: 3em;
    font-family: $font, sans-serif;
    opacity: 0.7;
}
h4 {
    margin-left: 70%;
    font-size: 3em;
    font-family: $font, sans-serif;
    opacity: 0.7;
    &.autre{
        margin-left: 5%;
    }
}


p{
    margin-left: 70%;
    font-size: 2em;
    font-family: $font, sans-serif;
    opacity: 0.7;
    &.autre{
    margin-left: 5%;
   }
}

.website{

    display: flex;
    flex-direction: row;
    justify-content: space-around;
    margin-left: 7%;
   img{
    width: 80%;
    border-radius: 10px; /* Bordure arrondie */
    border: solid 2px black; /* Bordure solid */

   }
}

@media screen and (max-width:730px){
    h4,h3,p{
        margin-left: 4%;
    }

    h4{
        font-size: 2.5em; 
    }
    p{
        font-size: 1.5em; 
    }
    h3{
        font-size: 3em;
    }
    
.website{

display: flex;
flex-direction: column;
justify-content: space-around;
margin-left: 7%;
img{
width: 80%;
border-radius: 10px; /* Bordure arrondie */
border: solid 2px black; /* Bordure solid */

}}

}


 }
</style>