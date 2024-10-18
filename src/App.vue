<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Sidebar from "@/components/Sidebar.vue";
import Navbar from "@/components/Navbar.vue";
</script>

<template>
  <div class="all">
    <Sidebar />
    <div class="main">
      <Navbar />
      <RouterView />
    </div>
  </div>
</template>

<style scoped>
.all {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  gap: 0;
}

.main {
  width: 80%;
  margin-left:20%;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  padding: 1rem;
}
</style>
