<script lang="ts">
    import me from '$lib/me.svg';
    import fleur from '$lib/fleure.svg';
    import fleurrond from '$lib/fleurrond.svg';
   
    // Définition de l'interface pour le type de données du réseau
    interface Reseau {
        competence: string; // Propriété pour stocker les compétences
    }

    // Déclaration du tableau de compétences
    let name: Reseau[] = [
        { competence: "software development" },
        { competence: "full stack" },
        { competence: "ui&ux designer" },
        { competence: "Marketing" },
        { competence: "Founder & CEO and CTO" }
    ];
</script>

<div class="competence">
<h2 >Skill</h2>

{#each name as { competence } }
    <h3> { competence } </h3>
    <div class="trait" role="presentation" aria-hidden="true"></div>
{/each}
<img src={fleurrond} alt="">
</div>


<div class="aboutme">
    <img  style="border-radius: 20px;"   src={fleur} alt="">
<h2>About me</h2>
<p>i'm Tyjust my real name is <br>
    thierry allou kouadio juste <br>
    im raised in ivoiry coast <br>
    and i lived in ivoiry coast and <br> 
    rwanda  i love create software <br>
    if is web app . desctop i love <br>
    juste create design me all reality <br>
    i’m a autodidact develloper  <br>
      </p>
      <div class="me">
      <img src={me} alt="my_picture"  width="500" height="500">
    </div>
</div>
<style lang="scss">
    @use "$lib/variable" as *;
   h3{
   
    font-size: 2em;
    font-family: $font, sans-serif;
    opacity: 0.6;
   }
   .trait {
    width: 20%;
    height: 1px;
    background-color: black;
    
}
h2{
    
    font-size: 2em;
    font-family: $font, sans-serif;
}
p{
   
    font-size: 2em;
    font-family: $font, sans-serif;
    opacity: 0.7;
}
.me{
    margin-left: -5%;
    display: flex;
    justify-content: center;
    align-items: cente;
}
.aboutme{
    margin-left: 5%;
    margin-top: -800px
  
}
.competence{
    margin-left: 70%;
}
@media screen and (max-width:1530px){
    h3{
   
   font-size: 1.8em;
   font-family: $font, sans-serif;
   opacity: 0.6;
  }
  .trait {
   width: 20%;
   height: 1px;
   background-color: black;
   
}
h2{
   
   font-size: 1.8em;
   font-family: $font, sans-serif;
}
p{
  
   font-size: 1.8em;
   font-family: $font, sans-serif;
   opacity: 0.7;
}
.me{
   margin-left: -5%;
}
.aboutme{
   margin-left: 5%;
   margin-top: -800px
 
}
.competence{
   margin-left: 70%;
}


        }


        @media screen and (max-width:730px){
    h3{
   
   font-size: 1.6em;
   font-family: $font, sans-serif;
   opacity: 0.6;
  }
  .trait {
   width: 20%;
   height: 1px;
   background-color: black;
   
}
h2{
   
   font-size: 1.6em;
   font-family: $font, sans-serif;
}
p{
  
   font-size: 1.6em;
   font-family: $font, sans-serif;
   opacity: 0.7;
}
.me{
   margin-left: -19%;
   
}
.aboutme{
   margin-left: 5%;
   margin-top: -200px
 
}
.competence{
   margin-left: 4%;
}


        }

</style>