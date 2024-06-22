<template>
  <q-layout view="hHh lpR fFf" class="app-layout">
    <q-header elevated class="bg-primary text-white">
      <q-toolbar>
        <q-toolbar-title>
          Tugas Paktikum Pemrograman Berbasis Komponen dari Pertemuan 1 hingga 7
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
.app-layout {
  min-height: 100vh;
  background-image: url('@/assets/pp2.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed; }

.bg-primary {
  background-color: #1976d2; 
}
</style>