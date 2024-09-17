<template>
  <header>
    <nav>
      <Disclosure as="nav" class="bg-gray-800 " v-slot="{ open }">
        <ul class="nav-link-wrap flex container">
          <div class="left">
            <DisclosureButton
              class="text-white uppercase [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
              ><NuxtLink to="/">HELPFUL</NuxtLink></DisclosureButton
            >
          </div>
          <div class="right">
            <li
              class="nav-link text-white uppercase [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
            >
              <NuxtLink to="/about">About</NuxtLink>
            </li>
            <li
              class="nav-link text-white uppercase [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
            >
              <NuxtLink to="/contact">Contact</NuxtLink>
            </li>
            <li
              class="nav-link text-white uppercase [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
            >
              <NuxtLink to="/login">Sign IN</NuxtLink>
            </li>
            <li
              class="btn-register text-white uppercase [item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
            >
              <NuxtLink to="/register">Register</NuxtLink>
            </li>
          </div>
        </ul>
      </Disclosure>
    </nav>
  </header>
</template>

<script setup>
import {
  Disclosure,
  DisclosureButton,
  DisclosurePanel,
  Menu,
  MenuButton,
  MenuItem,
  MenuItems,
} from "@headlessui/vue";
</script>

<style>
.btn-register {
  background-color: #a6f671;
  border-radius: 6px;
  color: #000000;
  font-size: 14px;
  font-weight: 700;
}

.container {
  margin: 0 auto;
  max-width: 1800px;
}

.nav-link-wrap {
  justify-content: space-between;
  padding: 10px 30px;
}

.nav-link {
  font-size: 14px;
  font-weight: 700;
  margin: 0 8px;
}

.right {
  display: flex;
}
</style>