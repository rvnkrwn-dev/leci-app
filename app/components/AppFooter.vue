<template>
  <footer class="text-center text-gray-500 mt-24 border-t border-gray-800 py-8">
    <p>&copy; {{ currentYear }} LECI Digital Solutions — Semua hak cipta dilindungi.</p>
    <p class="text-sm mt-2"><NuxtLink to="/privacy" class="hover:text-cyan-400">Kebijakan Privasi</NuxtLink> • <NuxtLink to="/terms" class="hover:text-cyan-400">Syarat & Ketentuan</NuxtLink></p>
  </footer>
</template>

<script setup lang="ts">
const currentYear = new Date().getFullYear();
</script>
