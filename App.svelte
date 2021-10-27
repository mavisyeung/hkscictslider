<script>
  import Button from "./Button.svelte";
  import Carousel from "./Carousel.svelte";
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
  <Carousel perPage="1">
    <div class="slide-content">
      <img alt="1" src="https://static.wixstatic.com/media/038890_0ff05eb9ea254be188cf0a1c4d36bf25~mv2.jpg/v1/fill/w_789,h_526,al_c,q_85,usm_0.66_1.00_0.01/038890_0ff05eb9ea254be188cf0a1c4d36bf25~mv2.webp"/>
    </div>
    <div class="slide-content">
      <img alt="2" src="https://static.wixstatic.com/media/038890_da367c978606423c87158638f849ac43~mv2.jpg/v1/fill/w_789,h_526,al_c,q_85,usm_0.66_1.00_0.01/038890_da367c978606423c87158638f849ac43~mv2.webp"/>
    </div>
    <div class="slide-content">
      <img alt="3" src="https://static.wixstatic.com/media/038890_07ea1f5cc2b94873b3408831cf195a4c~mv2.jpg/v1/fill/w_789,h_526,al_c,q_85,usm_0.66_1.00_0.01/038890_07ea1f5cc2b94873b3408831cf195a4c~mv2.webp"/>
    </div>
    <div class="slide-content">
      <img alt="4" src="https://static.wixstatic.com/media/038890_e6f6851b4d0f4934b17dcf28a29674a8~mv2.jpg/v1/fill/w_789,h_526,al_c,q_85,usm_0.66_1.00_0.01/038890_e6f6851b4d0f4934b17dcf28a29674a8~mv2.webp"/>
    </div>
  </Carousel>
</main>