<template>
  <nav class="sticky top-0 z-50 bg-opacity-80 backdrop-blur-lg border-b border-cyan-500/20" style="background-color: rgba(13, 2, 33, 0.8);">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        <!-- Logo -->
        <div class="grid grid-cols-2 items-center flex-shrink-0">
          <NuxtImg src="/leci.png" alt="leci" class="h-10" />
          <NuxtLink
              @click="scrollToTop"
              class="font-orbitron text-2xl font-bold text-white hover:text-cyan-400 transition-colors glitch"
              data-text="LECI"
          >
            LECI
          </NuxtLink>
        </div>
        <!-- Desktop Menu -->
        <div class="hidden md:block">
          <div class="ml-10 flex items-baseline space-x-8">
            <NuxtLink @click="scrollToSection('mengapa')" class="nav-link font-semibold cursor-pointer">Mengapa Kami</NuxtLink>
            <NuxtLink @click="scrollToSection('paket')" class="nav-link font-semibold cursor-pointer">Paket</NuxtLink>
            <NuxtLink @click="scrollToSection('proses')" class="nav-link font-semibold cursor-pointer">Proses</NuxtLink>
            <NuxtLink @click="scrollToSection('faq')" class="nav-link font-semibold cursor-pointer">FAQ</NuxtLink>
            <NuxtLink @click="scrollToSection('kontak')" class="cyber-btn text-sm cursor-pointer">Kontak</NuxtLink>
          </div>
        </div>
        <!-- Mobile Menu Button -->
        <div class="-mr-2 flex md:hidden">
          <button @click="toggleMobileMenu" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
            <span class="sr-only">Open main menu</span>
            <!-- Icon when menu is closed. -->
            <svg v-if="!isMobileMenuOpen" class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
            <!-- Icon when menu is open. -->
            <svg v-if="isMobileMenuOpen" class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <!-- Mobile menu, show/hide based on menu state. -->
    <div :class="{'block': isMobileMenuOpen, 'hidden': !isMobileMenuOpen}" class="md:hidden">
      <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
        <NuxtLink @click="handleMobileMenuClick('mengapa')" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium cursor-pointer">Mengapa Kami</NuxtLink>
        <NuxtLink @click="handleMobileMenuClick('paket')" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium cursor-pointer">Paket</NuxtLink>
        <NuxtLink @click="handleMobileMenuClick('proses')" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium cursor-pointer">Proses</NuxtLink>
        <NuxtLink @click="handleMobileMenuClick('faq')" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium cursor-pointer">FAQ</NuxtLink>
        <NuxtLink @click="handleMobileMenuClick('kontak')" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium cursor-pointer">Kontak</NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
// --- Reactive State ---
const isMobileMenuOpen = ref(false);

// --- Methods ---
const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};

const closeMobileMenu = () => {
  isMobileMenuOpen.value = false;
};

const scrollToSection = (sectionId: string) => {
  const element = document.getElementById(sectionId);
  if (element) {
    element.scrollIntoView({
      behavior: 'smooth',
      block: 'start',
      inline: 'nearest'
    });
  }
};

const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  });
};

const handleMobileMenuClick = (sectionId: string) => {
  closeMobileMenu();
  // Tambahkan slight delay untuk memastikan menu tertutup sebelum scroll
  setTimeout(() => {
    scrollToSection(sectionId);
  }, 100);
};
</script>