<template>
  <div class="min-h-screen">
    <AppHeader />
    <div class="w-full max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <slot />
    </div>
    <AppFooter />
  </div>
</template>

<script setup lang="ts">
import AppHeader from "~/components/AppHeader.vue";
import AppFooter from "~/components/AppFooter.vue";
</script>
