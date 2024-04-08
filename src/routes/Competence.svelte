
<script lang="ts">
    import svelteimg from "$lib/svelte.svg";
    import typescript from "$lib/typescript.svg";
    import supabase from "$lib/supabase.svg";
    import sql from "$lib/sql.svg";
    import figma from "$lib/figma.svg";
    import zig from "$lib/zig.svg";
    import bun from "$lib/bun.svg";
    import rust from "$lib/rust.svg";
     
  
   
</script>





<main >
    

    <h4>My favorite stack</h4>
    <h3>Javascript universe</h3>
   
        <div>
            <img src={svelteimg} alt='svelte_logo' width="120" height="120">  
            <img src={typescript} alt='typescript_logo' width="120" height="120">
        </div>
    



<h3>prostgest universe</h3>
<div>
    <img src={supabase} alt='supabase_logo' width="120" height="120">
    <img src={sql} alt='prosgres_logo' width="120" height="120">   
 </div>
<h3>Drizzle & figma</h3>
<div>
    <img src={figma} alt="figma_logo"  width="120" height="120">
    <img src={bun} alt="bun_logo"  width="120" height="120"> 
 </div>
<h3>bas niveau stack and runtime</h3>
<div>
    
      
    <img src={zig} alt="zig_logo"  width="120" height="120">    
    <img src={rust} alt="rust_logo"  width="120" height="120">   
        
 </div>

</main>

<style lang="scss">
    @use "$lib/variable" as *;
    @use "$lib/configue" as *;

    main{
        background-color: #122c5d;
        
       
        margin-top: 130px; /* Ajout d'une marge en haut */
        padding-bottom: 190px; /* Ajout d'une marge en bas */
        padding-top: 100px;
    /* le reste de votre code */
        div {
            border-radius: 10px; /* Bordure arrondie */
    box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.37); /* Ombre portée */
    width: 50%; /* Largeur de la div */
    margin: 0 auto; /* Centrage horizontal */
    display: flex;
    justify-content: space-between;
        flex-direction: columns;
        transition: ease-in 1s;
        background: rgba(255, 255, 255, 0.2); /* Couleur de fond avec opacité */
        &:hover{
        scale: 1.1;
        cursor: pointer;
        transition: ease-in 1s;
        background: rgba(255, 255, 255, 0.2); /* Couleur de fond avec opacité */
    backdrop-filter: blur(10px); /* Flou de l'arrière-plan */
    border-radius: 10px; /* Bordure arrondie */
    box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.37); /* Ombre portée */
    }
}
        
    
    h3{
        font-size: 2.7em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        opacity: 0.7;
        
    }
    /*.trait {
        width: 30%;
        height: 9px;
        background-color: black;
        @extend %div-center;
        margin-left: 35%;
        color: #D6E1FF;
        
        
    }*/
    h4{
        font-size: 3.2em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        
        
    }
    
   
    @media screen and (max-width:1330px){      
        div {
            border-radius: 10px; /* Bordure arrondie */
    box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.37); /* Ombre portée */
    width: 70%; /* Largeur de la div */
    margin: 0 auto; /* Centrage horizontal */
    display: flex;
    justify-content: space-between;
        flex-direction: row-reverse;
        transition: ease-in 1s;
       
     
}
h3{
        font-size: 2.1em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        opacity: 0.7;
        
    }


    h4{
        font-size: 2.6em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        
        
    }
    img{
        width: 80%;
    }

    }
    

    @media screen and (max-width:900px){
      
        div {
            border-radius: 10px; /* Bordure arrondie */
    box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.37); /* Ombre portée */
    width: 70%; /* Largeur de la div */
    margin: 0 auto; /* Centrage horizontal */
    display: flex;
    justify-content: space-between;
        flex-direction: row-reverse;
        transition: ease-in 1s;
       
     
}
h3{
        font-size: 1.9em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        opacity: 0.7;
        
    }


    h4{
        font-size: 2.4em;
        font-family: $font, sans-serif;
        text-align: center;
        color: #D6E1FF;
        
        
    }
    img{
        width: 70px;
    }

    }


    }
   


    
    </style>