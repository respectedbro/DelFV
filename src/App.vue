<template>
  <div class="page-wrapper">
    <Header @toggle-modal="isOpen = !isOpen" />
    <main class="main">
      <router-view></router-view>
    </main>
    <Modal :isOpen="isOpen" @toggle-modal="isOpen = !isOpen" />
    <Footer />
  </div>
</template>

<script setup>
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
import Modal from "@/components/Modal.vue";
import { ref } from "vue";

const isOpen = ref(false);
</script>

<style scoped></style>
