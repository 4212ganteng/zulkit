<script>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="md:order-2">
    <RouterLink
      to="/login"
      class="px-8 py-3 mt-2 mr-2 text-base font-medium text-black bg-gray-200 border border-transparent rounded-full hover:bg-gray-300 md:py-2 md:text-sm md:px-8 hover:shadow"
    >
      Sign In
    </RouterLink>
    <RouterLink
      to="/register"
      class="px-8 py-3 text-base font-medium text-white border border-transparent rounded-full bg-navy hover:bg-navy md:py-2 md:text-sm md:px-8 hover:shadow"
    >
      Sign Up
    </RouterLink>
  </div>
  <div
    class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1"
    id="mobile-menu-2"
  >
    <ul
      class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-regular"
    >
      <li>
        <RouterLink
          to="/"
          class="block py-2 pl-3 pr-4 text-white bg-indigo-600 rounded md:bg-transparent md:text-indigo-600 md:p-0 dark:text-white"
          aria-current="page"
          >Home</RouterLink
        >
      </li>
      <li>
        <RouterLink
          to="/category"
          class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
          >Categories</RouterLink
        >
      </li>
      <li>
        <RouterLink
          to="/pricing"
          href="#"
          class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
          >Pricing</RouterLink
        >
      </li>
      <li>
        <RouterLink
          to="/study-case"
          class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
          >Study Case</RouterLink
        >
      </li>
    </ul>
  </div>
</template>
