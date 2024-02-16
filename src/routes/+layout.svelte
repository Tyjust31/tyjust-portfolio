<script lang="ts">
  import { onMount } from 'svelte';
  import 'aos/dist/aos.css';
// @ts-ignore
  import AOS from "aos";


onMount(() => {
   AOS.init();


});
  let title: string = 'Tyjust\'s portfolio';
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";

  let y: number = 0;
  let bodyColor: string = '';

  onMount(() => {
    document.addEventListener('scroll', handleScroll);
    // Charger la dernière couleur depuis le stockage local lorsque la page est montée
    const savedColor = localStorage.getItem('bodyColor');
    if (savedColor) bodyColor = savedColor;
  });

  function handleScroll() {
    y = window.scrollY;

    if (y > 0 && y < 700) {
      bodyColor = '#FBDCEF';
    } else if (y > 700 && y < 1400) {
      bodyColor = '#D8D0BF';
    } else if (y > 1400 && y < 3100) {
      bodyColor = '#ACD8FC';
    } else if (y > 3100 && y < 5100) {
      bodyColor = '#CAF1F6';
    }else if (y > 5100 && y < 7100) {
      bodyColor = '#FFEFB8';
    }else if (y > 7100 && y < 9100) {
      bodyColor = '#ECCCFF';
    }
    // Sauvegarder la couleur actuelle dans le stockage local
    localStorage.setItem('bodyColor', bodyColor);
  }
</script>



<svelte:head>
  <title>{title}</title>
</svelte:head>



<body style="background-color: {bodyColor}; transition: background-color 0.5s ease-in-out;">
  <Header />
  <slot />
  <Footer />
</body>


<style lang="scss">
  body {
    margin: 0 auto;
    max-width: 2100px;
    scroll-behavior: smooth;
    overflow-x: hidden;
    background-color: #FFDCE1;
  }
</style>
