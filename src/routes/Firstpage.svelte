<script>
    import fleurplat from '$lib/fleurplat.svg';
</script>

<main>
    <div class="presentation">
        <h1>
            My name is Juste Allou <br>
            I love creating software<br>
            CEO of tech <br>
        </h1>
        <img class="fleur-img" src={fleurplat} alt="Fleur" />
        <div class="trait" role="presentation" aria-hidden="true"></div>
    </div>
    
</main>

<style lang="scss">
    @use "$lib/variable" as *;
    @use "$lib/configue" as *;

    main {
        .presentation {
           
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 120px;
                font-family: $font, sans-serif;
            }

            .trait {
                width: 90%;
                height: 3px;
                background-color: black;
                @extend %div-center;
            }
        }

        .fleur-img {
            margin-top: -610px;
            margin-left: 60%;
        }
        @media screen and (max-width: 1500px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 100px;
                font-family: $font, sans-serif;
            }

          
        }

        
        }
        @media screen and (max-width: 1230px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 80px;
                font-family: $font, sans-serif;
            }

          
        }

        
        }

        @media screen and (max-width: 970px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 60px;
                font-family: $font, sans-serif;
            }

          
        }

       
        }
      
        @media screen and (max-width: 750px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 50px;
                font-family: $font, sans-serif;
            }

          
        }

       
        }
        @media screen and (max-width: 610px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 42px;
                font-family: $font, sans-serif;
            }

          
        }

        
        }
        @media screen and (max-width: 510px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 35px;
                font-family: $font, sans-serif;
            }

          
        }

        
        }
        @media screen and (max-width: 430px){
            .presentation {
            position: relative;
            margin-left: 5%;

            h1 {
                color: #000000;
                font-size: 25px;
                font-family: $font, sans-serif;
            }

          
        }

        
        }
        
    }
    
</style>
