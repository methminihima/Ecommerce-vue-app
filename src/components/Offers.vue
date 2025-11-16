<template>
  <div id="offers" class="container scroll-mt-20 mx-auto px-4 py-12">
    <!-- Header -->
    <div class="text-center mb-12">
      <h2 class="text-3xl font-bold text-amber-900 mb-3">Special Offers</h2>
      <p class="text-lg text-gray-600">
        Take advantage of these limited-time offers
      </p>
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      <div
        v-for="offer in currentOffers"
        :key="offer.id"
        :class="[offer.bgColor,
            'rounded-xl shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105']"
        >
        <div class="p-6">
            <div class="flex justify-between items-start mb-4">
                <h3 :class="[offer.textColor,'text-xl font-semibold']">{{ offer.title }}</h3>
                <span class="bg-white rounded-full p-3 shadow-md">
                    <Icon :icon="offer.discount.includes('%') ? 'material-symbol:percent' :'mdi:gift'"
                    :class="[offer.textColor,'text-2xl']"/>
                </span>
            </div>
            <p class="text-gray-700 mb-4">{{ offer.description }}</p>
            <div class="flex item-center text-gray-600 mb-6">
                <Icon icon="svg-spinners:clock" class="mr-2" />
                <span>Ends on {{ offer.endDate }}</span>
            </div>
            <div class="bg-white rounded-lg p-4 mb-4">
                <p class="text-sm text-gray-500 mb-1">Use Code</p>
                <p class="font-bold font-mono text-lg">{{ offer.code }}</p>
            </div>

            <button :class="[offer.textColor,'w-full py-3 rounded-lg font-semibold border',
            offer.textColor.replace('text','border'),
            'hover:bg-white transition-colors duration-300']">Claim Offer</button>
        </div>
    </div>
      </div>
   
    </div>
</template>

<script setup>
import { ref } from 'vue'

const currentOffers = ref([
  {
    id: 1,
    title: 'Hot Summer Sale',
    description: 'Up to 30% off on our summer perfume collection',
    discount:'30%',
    endDate:'2024-07-31',
    code:'SUMMER30',
    bgColor:'bg-amber-200',
    textColor:'text-amber-700'
  },
  {
    id: 2,
    title: 'Free perfume Offer',
    description: 'Discover the latest fragrances just released this season',
    discount:'Gift',
    endDate:'2024-08-31',
    code:'FREEPERFUME',
    bgColor:'bg-purple-200',
    textColor:'text-Purple-700'
},
  {
    id: 3,
    title: 'New Launch Discount',
    description: 'Mix and match your favorite scents and save more',
    discount:'20%',
    endDate:'2024-07-31',
    code:'NEW20',
    bgColor:'bg-pink-200',
    textColor:'text-pink-700'
},
])
</script>

<style scoped>
/* Optional subtle hover effect */
</style>
