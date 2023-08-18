<template>
  <nav class="p-4">
    <div class="flex items-center justify-between px-2 lg:px-8">
      <!-- Logo atau Judul -->
      <div class="text-lg font-semibold text-slate-800">
        <h1 class="flex text-2xl font-bold items-center">SMK BP MARGASARI</h1>
      </div>

      <!-- Menu Toggle untuk Tampilan Mobile -->
      <div class="md:hidden">
        <button @click="toggleMenu" class="text-slate-800">
          <svg
            class="h-6 w-6"
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

      <!-- Menu untuk Tampilan Desktop -->
      <div class="hidden md:flex md:items-center md:space-x-4">
        <NuxtLink
          :to="{ name: 'index' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Home
        </NuxtLink>
        <NuxtLink
          :to="{ name: 'profile' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Profile
        </NuxtLink>
        <NuxtLink
          :to="{ name: 'blog' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Blog
        </NuxtLink>
        <NuxtLink
          :to="{ name: 'contact' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Contact
        </NuxtLink>
        <NuxtLink
          :to="{ name: 'ppdb-online' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          PPDB Online
        </NuxtLink>
      </div>
    </div>

    <!-- Menu untuk Tampilan Mobile -->
    <ul v-if="menuOpen" class="mt-4 md:hidden">
      <li class="flex">
        <NuxtLink
          :to="{ name: 'index' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Home
        </NuxtLink>
      </li>
      <li class="flex">
        <NuxtLink
          :to="{ name: 'profile' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Profile
        </NuxtLink>
      </li>
      <li class="flex">
        <NuxtLink
          :to="{ name: 'blog' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Blog
        </NuxtLink>
      </li>
      <li class="flex">
        <NuxtLink
          :to="{ name: 'contact' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          Contact
        </NuxtLink>
      </li>
      <li class="flex">
        <NuxtLink
          :to="{ name: 'ppdb-online' }"
          class="rounded-md px-3 py-2 font-medium text-slate-400 hover:bg-slate-800 hover:text-white"
        >
          PPDB Online
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menuOpen: false,
    }
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    },
  },
}
</script>
