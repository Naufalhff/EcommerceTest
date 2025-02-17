<template>
  <nav class="bg-white">
    <!-- Desktop Navigation -->
    <div class="hidden sm:block">
      <div class="grid grid-cols-12 border-b border-gray-200">
        <!-- Left Menu Items -->
        <div class="col-span-1 border-r border-gray-200">
          <nuxt-link
            to="/shop"
            class="block px-8 py-4 text-sm text-center text-gray-700 hover:text-gray-900"
          >
            Shop
          </nuxt-link>
        </div>
        <div class="col-span-1 border-r border-gray-200">
          <nuxt-link
            to="/contact"
            class="block px-8 py-4 text-sm text-center text-gray-700 hover:text-gray-900"
          >
            Contact
          </nuxt-link>
        </div>

        <!-- Empty Space -->
        <div class="col-span-7"></div>

        <!-- Right Menu Items with equal space and border at the edge -->
        <div class="col-span-1 border-l border-r border-gray-200">
          <nuxt-link
            to="/sign-in"
            class="block px-8 py-4 text-sm text-gray-700 hover:text-gray-900 text-center"
          >
            Sign in
          </nuxt-link>
        </div>
        <div class="col-span-1 border-r border-gray-200">
          <nuxt-link
            to="/cart"
            class="block px-8 py-4 text-sm text-gray-700 hover:text-gray-900 text-center"
          >
            Cart
          </nuxt-link>
        </div>
      </div>
    </div>

    <!-- Mobile Navigation -->
    <div class="sm:hidden">
      <!-- Mobile Menu Button -->
      <div class="border-b border-gray-200 px-4 py-3">
        <button
          @click="isOpen = !isOpen"
          class="flex items-center justify-between w-full"
        >
          <span class="text-sm">Menu</span>
          <svg
            class="h-5 w-5"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              v-if="!isOpen"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
            <path
              v-else
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M6 18L18 6M6 6l12 12"
            />
          </svg>
        </button>
      </div>

      <!-- Mobile Menu Content -->
      <div v-show="isOpen" class="border-b border-gray-200">
        <div class="divide-y divide-gray-200">
          <nuxt-link
            to="/shop"
            class="block px-4 py-3 text-sm text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            @click="isOpen = false"
          >
            Shop
          </nuxt-link>
          <nuxt-link
            to="/contact"
            class="block px-4 py-3 text-sm text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            @click="isOpen = false"
          >
            Contact
          </nuxt-link>
          <nuxt-link
            to="/sign-in"
            class="block px-4 py-3 text-sm text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            @click="isOpen = false"
          >
            Sign in
          </nuxt-link>
          <nuxt-link
            to="/cart"
            class="block px-4 py-3 text-sm text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            @click="isOpen = false"
          >
            Cart
          </nuxt-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";

const isOpen = ref(false);
</script>

<style scoped>
/* Optional: Remove default focus outline and add custom style */
</style>
