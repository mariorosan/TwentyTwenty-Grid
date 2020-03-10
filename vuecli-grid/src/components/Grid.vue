<template>
    <div class="container">
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-cat"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-hippo"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-dog"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-horse"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-paw"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-dove"></i>
          </span>
          <p>VueCLI Grid</p>
        </div>
      </div>                              
      <div class="box">
        <div class="content">
          <span style="font-size: 100px; color: #ffffff;">
            <i class="fas fa-fish"></i>
          </span>
          <p>VueCLI Grid</p>
        </div> 
      </div>                                                         
    </div>
</template>

<script>
export default {
  name: 'Grid',
}
</script>

<style>
   .container {
    position: relative;
    max-width: 100%;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    grid-template-rows: minmax(100px, auto);
    margin: 50px;
    grid-auto-flow: dense;
    grid-gap: 10px;
  }
  .box {
    background: #758aff;
    padding: 20px;
    display: grid;
    place-items: center;
    font-size: 25px;
    font-weight: 100;
    text-align: center;
    color: #fff;
    transition: 0.7s;
  }
  
  .box:hover {
    background: #21c8f6;
  }
  .box:nth-child(1) {
    grid-column: span 2;
    grid-row: span 1;
  }
  .box:nth-child(2) {
    grid-column: span 1;
    grid-row: span 2;
  }
  .box:nth-child(4) {
    grid-column: span 1;
    grid-row: span 2;
  }
  .box:nth-child(5) {
    grid-column: span 3;
    grid-row: span 1;
  }

  @media (max-width: 1036px) {
    .container {
      margin: 10px;
    }
  }

  @media (max-width: 840px) {
    .container {
      grid-template-columns: repeat(auto-fill, minmax(50%, 1fr));
      grid-template-rows: minmax(auto, auto);
      margin: 10px;
    }
    .box {
      grid-column: span 1 !Important;
      grid-row: span 1 !Important;
    }
  }
  
</style>


