<!-- components/common/Footer.vue -->
<template>
  <footer class="bg-gray-800 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div>
          <h3 class="text-lg font-semibold mb-4">Contact Us</h3>
          <ul class="space-y-2">
            <li>Email: info@kyivluxebouquets.com</li>
            <li>Phone: +380 44 123 4567</li>
            <li>Address: Kyiv, Ukraine</li>
          </ul>
        </div>

        <div>
          <h3 class="text-lg font-semibold mb-4">Quick Links</h3>
          <ul class="space-y-2">
            <li v-for="item in quickLinks" :key="item.path">
              <nuxt-link
                :to="item.path"
                class="hover:text-gray-300 transition-colors"
              >
                {{ item.name }}
              </nuxt-link>
            </li>
          </ul>
        </div>

        <div>
          <h3 class="text-lg font-semibold mb-4">Follow Us</h3>
          <div class="flex space-x-4">
            <a
              v-for="social in socialLinks"
              :key="social.name"
              :href="social.url"
              target="_blank"
              rel="noopener noreferrer"
              class="hover:text-gray-300 transition-colors"
            >
              {{ social.name }}
            </a>
          </div>
        </div>
      </div>

      <div class="mt-8 pt-8 border-t border-gray-700 text-center">
        <p>
          &copy; {{ new Date().getFullYear() }} Kyiv LuxeBouquets. All rights
          reserved.
        </p>
      </div>
    </div>
  </footer>
</template>

<script setup>
const quickLinks = [
  { name: "Fresh Flowers", path: "/fresh-flowers" },
  { name: "Dried Flowers", path: "/dried-flowers" },
  { name: "Live Plants", path: "/live-plants" },
  { name: "About Us", path: "/about" },
];

const socialLinks = [
  { name: "Instagram", url: "https://instagram.com" },
  { name: "Facebook", url: "https://facebook.com" },
  { name: "Twitter", url: "https://twitter.com" },
];
</script>
