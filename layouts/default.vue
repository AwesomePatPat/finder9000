
<script>
    import inputs from "../pages/inputs.vue";
</script>
<template>
<div class="header">
      <NuxtLink class="linkp" to="/">
        <svg xmlns="http://www.w3.org/2000/svg" width="75" height="75" fill="black" class="bi bi-emoji-heart-eyes" viewBox="0 0 16 16"><path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M11.315 10.014a.5.5 0 0 1 .548.736A4.498 4.498 0 0 1 7.965 13a4.498 4.498 0 0 1-3.898-2.25.5.5 0 0 1 .548-.736h.005l.017.005.067.015.252.055c.215.046.515.108.857.169.693.124 1.522.242 2.152.242.63 0 1.46-.118 2.152-.242a26.58 26.58 0 0 0 1.109-.224l.067-.015.017-.004.005-.002zM4.756 4.566c.763-1.424 4.02-.12.952 3.434-4.496-1.596-2.35-4.298-.952-3.434zm6.488 0c1.398-.864 3.544 1.838-.952 3.434-3.067-3.554.19-4.858.952-3.434z"/></svg>
      </NuxtLink>
      
      <div class="header-right">
        <NuxtLink class="linkp" to="/">
          <p class="active">Home</p>
        </NuxtLink>
        <NuxtLink class="linkp" to="/">
          <p>Contact</p>
        </NuxtLink>
        <NuxtLink class="linkp" to="/">
          <p>About</p>
        </NuxtLink>
    </div>
</div>
<div>
  <inputs />
</div>
</template>
<style>
/* Style the header with a grey background and some padding */
.header {
  overflow: hidden;
  background-color: #f1f1f1;
  padding: 5px 10px;
  font-family: 'Courier New', Courier, monospace;
}

/* Style the header links */
.header p {
  float: left;
  color: black;
  text-align: center;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  line-height: 25px;
  border-radius: 4px;
}

/* Style the logo link (notice that we set the same value of line-height and font-size to prevent the header to increase when the font gets bigger */
.header svg.logo {
  font-size: 25px;
  font-weight: bold;
}

/* Change the background color on mouse-over */
.header p:hover {
  background-color: #ddd;
  color: black;
}

/* Style the active/current link*/
.header p.active {
  background-color: dodgerblue;
  color: white;
}

.header p.active:hover {
  background-color: rgb(74, 164, 255);
  color: white;
}

/* Float the link section to the right */
.header-right {
  float: right;
}

/* Add media queries for responsiveness - when the screen is 500px wide or less, stack the links on top of each other */
@media screen and (max-width: 500px) {
  .header p {
    float: none;
    display: block;
    text-align: left;
  }
  .header-right {
    float: none;
  }
}



</style>