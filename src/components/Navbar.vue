<template>
  <div>
    <!-- Navbar -->
    <div
      id="navbar"
      class="w-full h-[90px] fixed top-0 left-0 z-20 px-4 py-3 transition-colors duration-100 bg-transparent text-white font-semibold"
    >
      <div class="max-w-screen-xl mx-auto flex justify-between items-center">
        <div class="flex items-center space-x-3">
          <img src="../assets/images/logo.png" alt="Logo" class="w-8 h-8" />
          <p id="logotext" class="text-xl font-bold">Startup Landing</p>
        </div>

        <!-- Desktop Nav -->
        <nav class="hidden lg:flex space-x-8">
          <router-link to="#home">Home</router-link>
          <router-link to="#features">Features</router-link>
          <router-link to="#testimonial">Testimonial</router-link>
          <router-link to="#pricing">Pricing</router-link>
        </nav>

        <button
          class=" border border-white rounded-full w-[150px] h-[46px] hover:bg-white hover:text-black"
        >
          Get Started
        </button>

        <button @click="toggleMenu" class="lg:hidden z-30">
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            ></path>
          </svg>
        </button>
      </div>
    </div>
<!-- mobile nav -->
    <div
      class="fixed top-0 left-0 h-full w-64 bg-white text-black transform transition-transform duration-300 z-20 lg:hidden"
      :class="{ '-translate-x-full': !menuOpen, 'translate-x-0': menuOpen }"
    >
      <div class="p-6 space-y-6 mt-20">
        <router-link to="#home" @click="closeMenu" class="block">Home</router-link>
        <router-link to="#features" @click="closeMenu" class="block">Features</router-link>
        <router-link to="#testimonial" @click="closeMenu" class="block">Testimonial</router-link>
        <router-link to="#pricing" @click="closeMenu" class="block">Pricing</router-link>
        
      </div>
    </div>

    <div
      v-if="menuOpen"
      @click="closeMenu"
      class="fixed inset-0 bg-black opacity-20 z-10 lg:hidden"
    ></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
    closeMenu() {
      this.menuOpen = false;
    },
  },
};
</script>
