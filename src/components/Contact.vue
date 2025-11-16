<template>
  <div
    id="contact"
    class="min-h-screen scroll-mt-20 bg-[#4a0028] text-white py-16 px-6 sm:px-10 lg:px-20"
  >
    <div class="max-w-7xl mx-auto">
      <div class="text-center mb-12">
        <h2 class="text-4xl font-bold text-pink-300 mb-3">Get in Touch</h2>
        <p class="text-gray-200">
          Have questions about our perfumes? Our fragrance experts are here to help you.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-10">
        <!-- Contact Form -->
        <div class="bg-white text-gray-800 rounded-2xl p-8 shadow-lg">
          <h3 class="text-2xl font-semibold mb-6">Send Us a Message</h3>

          <form class="space-y-5">
            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1"
                >Your Name</label
              >
              <input
                type="text"
                placeholder="Your name"
                class="w-full border border-gray-300 rounded-md p-3 focus:ring-2 focus:ring-pink-500 focus:outline-none"
              />
            </div>

            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1"
                >Email Address</label
              >
              <input
                type="email"
                placeholder="Your@email.com"
                class="w-full border border-gray-300 rounded-md p-3 focus:ring-2 focus:ring-pink-500 focus:outline-none"
              />
            </div>

            <div>
              <label class="block text-sm font-medium text-gray-700 mb-1"
                >Your Message</label
              >
              <textarea
                rows="4"
                placeholder="Tell us about your fragrance needs..."
                class="w-full border border-gray-300 rounded-md p-3 focus:ring-2 focus:ring-pink-500 focus:outline-none"
              ></textarea>
            </div>

            <button
              type="submit"
              class="w-full bg-pink-700 text-white font-semibold py-3 rounded-md hover:bg-pink-800 transition"
            >
              Send Message
            </button>
          </form>
        </div>

        <!-- Contact Info -->
        <div class="bg-white text-gray-800 rounded-2xl p-8 shadow-lg">
          <h3 class="text-2xl font-semibold mb-6">Contact Information</h3>

          <ul class="space-y-6">
            <li class="flex items-start gap-4">
              <div
                class="bg-pink-100 text-pink-600 p-3 rounded-full flex items-center justify-center"
              >
                <i class="fas fa-phone-alt"></i>
              </div>
              <div>
                <h4 class="font-semibold text-gray-900">Phone</h4>
                <p class="text-gray-600">+1 (234) 567-8900</p>
                <p class="text-gray-500 text-sm">Mon–Fri: 9am–6pm</p>
              </div>
            </li>

            <li class="flex items-start gap-4">
              <div
                class="bg-pink-100 text-pink-600 p-3 rounded-full flex items-center justify-center"
              >
                <i class="fas fa-envelope"></i>
              </div>
              <div>
                <h4 class="font-semibold text-gray-900">Email</h4>
                <p class="text-gray-600">contact@perfumelux.com</p>
                <p class="text-gray-600">support@perfumelux.com</p>
              </div>
            </li>

            <li class="flex items-start gap-4">
              <div
                class="bg-pink-100 text-pink-600 p-3 rounded-full flex items-center justify-center"
              >
                <i class="fas fa-map-marker-alt"></i>
              </div>
              <div>
                <h4 class="font-semibold text-gray-900">Our Boutique</h4>
                <p class="text-gray-600">123 Perfume Street</p>
                <p class="text-gray-600">Paris, France 75001</p>
              </div>
            </li>
          </ul>
              <!-- Follow Us Section -->
          <div class="mt-10 border-t border-gray-200 pt-6">
            <h4 class="font-semibold text-gray-900 mb-4">Follow Us</h4>
            <div class="flex gap-4">
              <a
                href="#"
                class="bg-pink-100 text-pink-600 p-3 rounded-full hover:bg-pink-200 transition"
              >
                <i class="fab fa-facebook-f"></i>
              </a>
              <a
                href="#"
                class="bg-pink-100 text-pink-600 p-3 rounded-full hover:bg-pink-200 transition"
              >
                <i class="fab fa-twitter"></i>
              </a>
              <a
                href="#"
                class="bg-pink-100 text-pink-600 p-3 rounded-full hover:bg-pink-200 transition"
              >
                <i class="fab fa-instagram"></i>
              </a>
              <a
                href="#"
                class="bg-pink-100 text-pink-600 p-3 rounded-full hover:bg-pink-200 transition"
              >
                <i class="fab fa-linkedin-in"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// No special imports needed; Font Awesome icons can be used globally if added in main.js
</script>

<style scoped>
/* optional: adjust icons if using Font Awesome CDN */
i {
  font-size: 1.25rem;
}
</style>
