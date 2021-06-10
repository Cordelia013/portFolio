<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
    <img :src="calculatedImgURL" alt="">
  </div>
</template>