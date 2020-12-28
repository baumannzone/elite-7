<template>
  <!-- This example requires Tailwind CSS v2.0+ -->
  <nav class="bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex items-center">
          <div class="flex-shrink-0">
            <img
              class="block h-8 w-auto"
              src="/elite7-blanco.png"
              alt="Elite 7 Asesor"
            />
          </div>
          <div class="hidden sm:block sm:ml-6">
            <div class="flex space-x-4">
              <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
              <a
                v-for="item in navItems"
                :key="item.displayText"
                href="#"
                class="text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-blue-500"
                >{{ item.displayText }}</a
              >
            </div>
          </div>
        </div>
        <div class="hidden sm:ml-6 sm:block"></div>
        <div class="-mr-2 flex sm:hidden">
          <!-- Mobile menu button -->
          <button
            class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-insest focus:ring-white"
            aria-expanded="false"
            @click="showMenu = !showMenu"
          >
            <span class="sr-only">Open main menu</span>
            <!-- Icon when menu is closed. -->
            <!--
              Heroicon name: menu
              Menu open: "hidden", Menu closed: "block"
            -->
            <svg
              :class="showMenu ? 'hidden' : 'block'"
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
            <!-- Icon when menu is open. -->
            <!--
              Heroicon name: x
              Menu open: "block", Menu closed: "hidden"
            -->
            <svg
              :class="showMenu ? 'block' : 'hidden'"
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <!--
      Mobile menu, toggle classes based on menu state.
      Menu open: "block", Menu closed: "hidden"
    -->
    <transition
      enter-active-class="transition ease-out duration-100"
      enter-class="transform opacity-0 scale-95"
      enter-to-class="transform opacity-100 scale-100"
      leave-active-class="transition ease-in duration-75"
      leave-class="transform opacity-100 scale-100"
      leave-to-class="transform opacity-0 scale-95"
    >
      <!--
        Entering: "transition ease-out duration-100"
        From: "transform opacity-0 scale-95"
        To: "transform opacity-100 scale-100"
        Leaving: "transition ease-in duration-75"
        From: "transform opacity-100 scale-100"
        To: "transform opacity-0 scale-95"
       -->
      <div v-show="showMenu">
        <div class="px-2 pt-2 pb-3 space-y-1">
          <!--
          Current: "bg-gray-900 text-white",
          Default: "text-gray-300 hover:bg-gray-700 hover:text-white"
        -->
          <a
            v-for="item in navItems"
            :key="item.displayText"
            href="#"
            class="block text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-gray-700 hover:text-white"
          >
            {{ item.displayText }}
          </a>
          <!-- <a
         class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
        </a>-->
        </div>
      </div>
    </transition>
  </nav>
</template>

<script>
const navItems = [
  { displayText: 'Inicio' },
  { displayText: 'Servicios' },
  { displayText: 'Quiénes Somos' },
  { displayText: 'Contacto' },
]
export default {
  name: 'NavigationBar',
  data() {
    return {
      navItems,
      showMenu: false,
    }
  },
}
</script>
