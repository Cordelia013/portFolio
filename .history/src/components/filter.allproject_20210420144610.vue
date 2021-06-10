<template>
  <div class="project">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
    <img :src="calculatedImgURL" alt="">
  </div>
</template>