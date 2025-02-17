<!-- layouts/default.vue -->
<template>
  <div class="min-h-screen bg-gray-50">
    <Navbar />
    <main>
      <slot />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from "~/components/common/Navbar.vue";
import Footer from "~/components/common/Footer.vue";
</script>
