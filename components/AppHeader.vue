<template>
    <header>
      <nav>
        <Disclosure as="nav" class="bg-gray-800" v-slot="{ open }">
        <ul class="flex">
          <DisclosureButton  class="text-white [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"><NuxtLink to="/">Home</NuxtLink></DisclosureButton>
          <li class="text-white [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"><NuxtLink to="/about">About</NuxtLink></li>
          <li class="text-white [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"><NuxtLink to="/product">Product</NuxtLink></li>
        </ul>
        </Disclosure>
      </nav>
    </header>
  </template>
  
  <script setup>
import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'

</script>