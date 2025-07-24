<template>
  <div class="slidev-layout default">
    <slot />
    <Footer />
  </div>
</template>

<script setup>
import Footer from '../components/Footer.vue'
</script>

<style>
.slidev-layout.default {
  padding-bottom: 80px; /* Make room for the footer */
}
</style> 