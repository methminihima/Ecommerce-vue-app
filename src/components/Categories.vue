<template>
  <section id="categories" class="py-16 scroll-mt-20 bg-white">
    <div class="container mx-auto px-4">
      <!-- Section Header -->
      <div class="text-center mb-12">
        <h2 class="text-3xl font-bold text-amber-950 mb-3">
          Explore Our Fragrance Collections
        </h2>
        <p class="text-lg text-gray-800 max-w-2xl mx-auto">
          Discover scents that match your personality
        </p>
      </div>

      <!-- Categories Grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <div
          v-for="(category, index) in categories"
          :key="index"
          class="relative group rounded-lg shadow-md overflow-hidden hover:lg transition-transform-shadow duration-300"
        >
        <div class="h-64 overflow-hidden">
            <img :src="category.image":alt="category.alt"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
        </div>
        <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent">
            <div class="absolute bottom-0 left-0 p-6">
                <h3 class="text-white text-xl font-semibold">{{ category.title }}</h3>
                <p class="text-gray-200 mt-1">{{ category.description }}</p>
            </div>
        </div>
           
    </div>
      </div>
    </div>
  </section>
</template>

<script setup>

import { ref } from 'vue';
import product8 from '../assets/Image 1.jpg'
import product9 from '../assets/Image2.jpg'
import product10 from '../assets/Image3.jpg'
import product11 from '../assets/Image4.jpg'
import product12 from '../assets/Image5.jpg'
import product13 from '../assets/Image6.jpg'

const categories =ref([
    {image:product8,title:"Men's Collection",description:"Bold and masculine fragrances for modern men.",alt:"Men's Collection"},
    {image:product8,title:"Women's Collection",description:"Elegant, timeless scents crafted for confident women.",alt:"Women's Collection"},
    {image:product8,title:"Luxury Collection",description:"Premium designer perfumes for a lavish experience.",alt:"Luxury Collection"},
    {image:product8,title:"Gift Sets",description:"Perfect fragrance bundles for every special occasion.",alt:"Gift Sets"},
    {image:product8,title:"Trending Scents",description:"Top-selling perfumes loved by our customers right now.",alt:"Trending Scents"},
    {image:product8,title:"New Arrivals",description:"Fresh, new fragrances recently added to our collection.",alt:"New Arrivals"},
])

</script>
