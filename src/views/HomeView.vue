<template>
    <HeaderComponent />
    <section>
      <MDBCarousel
        v-model="carousel4" 
        :items="items4"
        fade
      />
    </section>
    <FooterComponent />
</template>

<script setup lang="ts">
  import { MDBCarousel } from 'mdb-vue-ui-kit';
  import FooterComponent from '../components/FooterComponent.vue';
  import HeaderComponent from '../components/HeaderComponent.vue';
  import { ref } from 'vue';
  
  const items4 = [
  {
      src: "https://mdbootstrap.com/img/Photos/Slides/img%20(15).webp",
      alt: "..."
    },
    {
      src: "https://mdbootstrap.com/img/Photos/Slides/img%20(22).webp",
      alt: "..."
    },
    {
      src: "https://mdbootstrap.com/img/Photos/Slides/img%20(23).webp",
      alt: "..."
    }
  ];
  const carousel4 = ref(0)
</script>

<style scoped>
</style>
