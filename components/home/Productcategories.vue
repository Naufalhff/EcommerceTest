<!-- components/home/ProductCategories.vue -->
<template>
  <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
    <div
      v-for="category in categories"
      :key="category.id"
      class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow"
    >
      <nuxt-link :to="category.path">
        <div class="relative h-64">
          <img
            :src="category.image"
            :alt="category.name"
            class="w-full h-full object-cover"
          />
        </div>
        <div class="p-6">
          <h3 class="text-xl font-semibold text-gray-900 mb-2">
            {{ category.name }}
          </h3>
          <p class="text-gray-600">{{ category.description }}</p>
        </div>
      </nuxt-link>
    </div>
  </section>
</template>

<script setup>
const categories = [
  {
    id: 1,
    name: "Fresh Flowers",
    description: "Beautiful, hand-picked fresh flowers for any occasion",
    image: "#",
    path: "#",
  },
  {
    id: 2,
    name: "Dried Flowers",
    description: "Long-lasting dried flower arrangements",
    image: "#",
    path: "#",
  },
  {
    id: 3,
    name: "Live Plants",
    description: "Indoor plants to bring life to your space",
    image: "#",
    path: "#",
  },
];
</script>
