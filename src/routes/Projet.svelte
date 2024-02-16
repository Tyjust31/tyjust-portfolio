<script lang="ts">
   import mode from "$lib/mode.svg";
   import violet from "$lib/violet.svg";
   import sport from "$lib/sport.svg";
   import moon from "$lib/moon.svg";
   import light from "$lib/light.svg";
   import kenneth from "$lib/kenneth.svg";
   import modeb from "$lib/modeb.svg";
   import davix from "$lib/davix.svg";
   import saintv from "$lib/saintv.svg";
   import app from "$lib/app.svg";

   interface website {
    src: string;
     alt: string;
     href: string;
   }

   let name: website[] = [
    { src: mode, alt: "logo mode", href: "https://mode.com" },
      { src: violet, alt: "logo violet", href: "https://violet.com" },
      { src: sport, alt: "logo sport", href: "https://sport.com" },
      ]

      let figma: website[] = [
    { src: mode, alt: "logo mode", href: "https://mode.com" },
      { src: saintv, alt: "logo violet", href: "https://violet.com" },
      { src: app, alt: "logo sport", href: "https://sport.com" },
      ]

      let logo: website[] = [
    { src: davix, alt: "logo mode", href: "https://mode.com" },
      { src: kenneth, alt: "logo violet", href: "https://violet.com" },
      { src: moon, alt: "logo sport", href: "https://sport.com" },
      ]
</script>



<main>

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