<script>
  import Button from "./Button.svelte";
  import Carousel from "./Carousel.svelte";
  let isShown = false;
  let images = [
    "https://i.imgur.com/UD0p9FO.jpg",
    "https://i.imgur.com/KRZp1J9.jpg",
    "https://static.wixstatic.com/media/038890_07ea1f5cc2b94873b3408831cf195a4c~mv2.jpg/v1/fill/w_789,h_526,al_c,q_85,usm_0.66_1.00_0.01/038890_07ea1f5cc2b94873b3408831cf195a4c~mv2.webp"
  ];
  let hue = 4698;
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }

  .slide-content img {
    height: 50vh;
  }
</style>

<main>
	<h1>Hello CodeSandbox</h1>
	<h2>Start editing to see some magic happen!</h2>
	<Button />
  <br>
  <br>
  {#if isShown}
  <Carousel perPage="1">
   {#each images as image, i}
    <div class="slide-content">
      <img alt="1" src={image}/>
   
    </div>
   {/each}
  </Carousel>
  {:else}
  <div on:click={() => isShown=true}
       on:mousemove={e => hue = e.clientX * e.clientY}
       style="background: hsl({hue/500}, 100%, 50%); height:50vh"/>
  
  {/if}
</main>