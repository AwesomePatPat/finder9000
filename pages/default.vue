<template>
<div class="header">
      <NuxtLink class="linkp" to="/">
        <p class="logo">CompanyLogo</p>
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
.header p.logo {
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