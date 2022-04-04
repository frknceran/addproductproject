<template>
<div class="flex md:container md:mx-auto mt-6"> 
<div class="carousel w-full">
  <div id="slide1" class="carousel-item relative w-full">
    <img src="../assets/image 324.png" class="w-full"> 
    <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
      <a href="#slide4" class="btn btn-circle">❮</a> 
      <a href="#slide2" class="btn btn-circle">❯</a>
    </div>
  </div> 
</div>
</div>
</template>
<script>
export default {
    name: 'appCarousel',
}
</script>