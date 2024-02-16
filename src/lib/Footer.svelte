<script lang="ts">
    import google from "$lib/googel.svg";
    import fb from "$lib/facebook.svg";
    import lin from "$lib/lin.svg";
    import x from "$lib/x.svg";
    import insta from "$lib/instagram.svg"
    import github from "$lib/github.svg"
  
    interface Reseau {
      src: string;
      alt: string;
      href?: string;
    }
  
    let name: Reseau[] = [
      { src: google, alt: "logo googel", href: "https://google.com" },
      { src: fb, alt: "logo facebook", href: "https://facebook.com" },  
      { src: lin, alt: "logo linkdin", href: "https://linkedin.com" },
      { src: x, alt: "logo x", href: "https://twitter.com/Tyjust31" },
      { src: insta, alt: "logo intagrame", href: "https://www.instagram.com/tyjust31/" },
      { src: github, alt: "logo github", href: "https://github.com/Tyjust31" },
    ];
  </script>
  
  
    
  <main>
    <h4 >Contact</h4>
    <div class="reseau">
      {#each name as { src, alt, href }}
        {#if typeof href === "string"}
          <a   {href}><img {src} {alt} /></a>
        {:else}
          <img {src} {alt} />
        {/if}
      {/each}
    </div>
  
 
    

    <p>👨🏿 <br>see you again</p>


    <h3  >
      Designed and built by 'Juste ALLOU'
      <span>&copy; Copyright 2024 - Juste ALLOU</span>
    </h3>
  
    <hr />
    <p>i'm the best developer in the world</p>
     
    <h4>you alwayse there :)</h4>
    </main>
    
    <style lang="scss">
      @use "$lib/variable" as *;
      @use "$lib/lastfont" as *;
      main {
            

        h4 {
          margin-top: 50px;
          text-align: center;
          font-size: 2em;
          font-family: $font;
          font-weight: 300;
        }
    
        .reseau {
          display: grid;
        grid-template-columns: repeat(6, 1fr);
        grid-template-rows: repeat(6, 1fr);
        grid-gap: 5px;
          place-items: center;
          justify-content: center;
          align-items: center;
          height: 100px;
         
        }
    
        h3 {
          font-family: $font;
          font-size: 2em;
          text-align: center;
        }
        a{
            img{
               width: 70px;
               
            }
        }
       
      }
   p{
    font-size: 12em;
    font-family: $fontlayout;
    margin-left: 50%;
   }



   @media screen and (max-width:560px){
    main{
     .reseau{
      grid-template-columns: repeat(3, 1fr);
                grid-template-rows: repeat(3, 1fr);
                grid-gap: 5px;
                place-items: center;
                justify-content: center;
                align-items: center;
                height: 100px;

            }
          h3{
            font-size: 1.5em;
     }
     p{
      font-size: 6em;
        margin-left: 5%;
     }
    }
}

    </style>
  