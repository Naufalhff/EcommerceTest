<!-- pages/index.vue -->
<template>
  <div class="grid grid-cols-12">
    <!-- Left Section -->
    <div class="col-span-6 p-8 border-r border-gray-200 ml-2">
      <div class="mb-8">
        <h1 class="text-3xl font-bold mb-2">Kyiv LuxeBouquets®</h1>
        <p class="text-sm text-gray-600">
          Discover Uniquely Crafted Bouquets and Gifts for Any Occasion
        </p>
      </div>

      <div class="grid grid-cols-2 gap-4">
        <div class="relative">
          <img
            src="../assets/images/bunga1.jpg"
            alt="Florist at work"
            class="w-full h-48 object-cover"
          />
        </div>
        <div class="flex items-center">
          <p class="text-sm text-gray-600">
            Experience the joy of giving with our carefully crafted bouquets
            designed to make every moment special
          </p>
        </div>
      </div>
    </div>

    <!-- Right Section -->
    <div class="col-span-6 border-l border-gray-200">
      <div class="grid grid-cols-2">
        <!-- Fresh Flowers -->
        <div class="border-b border-r border-gray-200 p-6">
          <h2 class="text-lg font-medium mb-4">Fresh Flowers</h2>
          <div class="flex justify-between items-center">
            <span class="text-sm">Shop now →</span>
          </div>
        </div>
        <div class="border-b border-gray-200">
          <img
            src="../assets/images/bunga2.jpg"
            alt="Fresh Flowers"
            class="w-full h-48 object-cover"
          />
        </div>

        <!-- Dried Flowers -->
        <div class="border-b border-r border-gray-200 p-6">
          <h2 class="text-lg font-medium mb-4">Dried Flowers</h2>
          <div class="flex justify-between items-center">
            <span class="text-sm">← Shop now</span>
          </div>
        </div>
        <div class="border-b border-gray-200">
          <img
            src="../assets/images/bunga3.jpg"
            alt="Dried Flowers"
            class="w-full h-48 object-cover"
          />
        </div>

        <!-- Live Plants -->
        <div class="border-b border-r border-gray-200 p-6">
          <h2 class="text-lg font-medium mb-4">Live Plants</h2>
          <div class="flex justify-between items-center">
            <span class="text-sm">Shop now →</span>
          </div>
        </div>
        <div class="border-b border-gray-200">
          <img
            src="../assets/images/bunga3.jpg"
            alt="Live Plants"
            class="w-full h-48 object-cover"
          />
        </div>

        <!-- Aroma Candles -->
        <div class="border-b border-r border-gray-200 p-6">
          <h2 class="text-lg font-medium mb-4">Aroma Candles</h2>
          <div class="flex justify-between items-center">
            <span class="text-sm">Shop now →</span>
          </div>
        </div>
        <div class="border-b border-gray-200">
          <img
            src="../assets/images/bunga4.jpg"
            alt="Aroma Candles"
            class="w-full h-48 object-cover"
          />
        </div>

        <!-- Fresheners -->
        <div class="border-r border-gray-200 p-6">
          <h2 class="text-lg font-medium mb-4">Fresheners</h2>
          <div class="flex justify-between items-center">
            <span class="text-sm">Shop now →</span>
          </div>
        </div>
        <div>
          <img
            src="../assets/images/bunga5.jpg"
            alt="Fresheners"
            class="w-full h-48 object-cover"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional scripts needed for now
</script>
