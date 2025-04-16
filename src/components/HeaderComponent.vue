<template>
  <header class="header">
    <MDBNavbar light bg="light" expand="lg" container>
      <MDBNavbarToggler
        target="#navbarNav"
        @click="collapse2 = !collapse2"
      ></MDBNavbarToggler>
      <MDBCollapse id="navbarNav" v-model="collapse2">
        <MDBNavbarNav center class="text-uppercase">
          <MDBNavbarItem to="#">Inicio </MDBNavbarItem>
          <MDBNavbarItem to="#"> Nosotros </MDBNavbarItem>
          <MDBNavbarItem to="#"> Productos </MDBNavbarItem>
          <MDBNavbarItem to="#"> Contacto </MDBNavbarItem>
          <MDBNavbarItem to="#"> Recursos </MDBNavbarItem>
        </MDBNavbarNav>
      </MDBCollapse>
    </MDBNavbar>
  </header>
</template>

<script setup lang="ts">
    import {
        MDBNavbar,
        MDBNavbarToggler,
        MDBNavbarNav,
        MDBNavbarItem,
        MDBCollapse,
    } from 'mdb-vue-ui-kit';
    import { ref } from 'vue';

    const collapse2 = ref(false);
</script>

<style scoped>

  .header{
    font-family: "Montserrat", sans-serif !important;
  }

  :deep(.nav-link) {
  color: #2A7C6F !important; /* tu color personalizado */
}

</style>
