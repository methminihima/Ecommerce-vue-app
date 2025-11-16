<template>
  <footer class="bg-pink-950 text-white mt-12">
    <!-- Top Footer -->
    <div class="max-w-7xl mx-auto px-6 py-10 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10">

      <!-- Brand -->
      <div>
        <h2 class="text-2xl font-bold text-pink-300">ShopEase</h2>
        <p class="text-gray-300 mt-3 text-sm leading-relaxed">
          Your trusted destination for luxury perfumes, beauty essentials, and exclusive deals.
        </p>

        <!-- Social Icons -->
        <div class="flex space-x-4 mt-4">
          <a href="#" class="text-gray-300 hover:text-pink-300">
            <Icon icon="mdi:facebook" class="w-6 h-6" />
          </a>
          <a href="#" class="text-gray-300 hover:text-pink-300">
            <Icon icon="mdi:instagram" class="w-6 h-6" />
          </a>
          <a href="#" class="text-gray-300 hover:text-pink-300">
            <Icon icon="mdi:twitter" class="w-6 h-6" />
          </a>
        </div>
      </div>

      <!-- Quick Links -->
      <div>
        <h3 class="font-semibold text-lg text-pink-200 mb-3">Quick Links</h3>
        <ul class="space-y-2 text-gray-300 text-sm">
          <li><a href="#home" class="hover:text-pink-300">Home</a></li>
          <li><a href="#products" class="hover:text-pink-300">Products</a></li>
          <li><a href="#categories" class="hover:text-pink-300">Categories</a></li>
          <li><a href="#offers" class="hover:text-pink-300">Offers</a></li>
        </ul>
      </div>

      <!-- Support -->
      <div>
        <h3 class="font-semibold text-lg text-pink-200 mb-3">Support</h3>
        <ul class="space-y-2 text-gray-300 text-sm">
          <li><a href="#about" class="hover:text-pink-300">About Us</a></li>
          <li><a href="#contact" class="hover:text-pink-300">Contact</a></li>
          <li><a href="#" class="hover:text-pink-300">FAQs</a></li>
          <li><a href="#" class="hover:text-pink-300">Shipping Info</a></li>
        </ul>
      </div>

      <!-- Newsletter -->
      <div>
        <h3 class="font-semibold text-lg text-pink-200 mb-3">Stay Updated</h3>
        <p class="text-gray-300 text-sm">Subscribe to get the latest offers and updates.</p>

        <div class="flex mt-4">
          <input
            type="email"
            placeholder="Enter your email"
            class="w-full px-3 py-2 rounded-l-lg bg-white/10 text-white placeholder-gray-300 outline-none focus:ring-2 focus:ring-pink-400"
          />
          <button class="px-4 bg-pink-600 hover:bg-pink-500 rounded-r-lg text-white">
            <Icon icon="mdi:send" class="w-5 h-5" />
          </button>
        </div>
      </div>

    </div>

    <!-- Bottom Footer -->
    <div class="bg-pink-900 py-4">
      <p class="text-center text-gray-300 text-sm">
        © {{ new Date().getFullYear() }} ShopEase. All rights reserved.
      </p>
    </div>
  </footer>
</template>

<script setup>
import { Icon } from "@iconify/vue";
</script>
