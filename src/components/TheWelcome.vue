<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="flex flex-col rounded-md shadow-sm md:inline-flex md:flex-row">
    <RouterLink to="/job-board">
      <button
        type="button"
        class="inline-flex items-center justify-center gap-2 px-4 py-3 -mt-px -ml-px text-sm font-medium text-gray-700 align-middle transition-all bg-white border first:rounded-t-lg last:rounded-b-lg sm:first:rounded-l-lg sm:mt-0 sm:first:ml-0 sm:first:rounded-tr-none sm:last:rounded-bl-none sm:last:rounded-r-lg hover:bg-gray-50 focus:z-10 focus:outline-none focus:ring-2 focus:ring-blue-600 dark:bg-gray-800 dark:hover:bg-slate-800 dark:border-gray-700 dark:text-gray-400"
      >
        Find jobs
      </button>
    </RouterLink>
    <RouterLink to="/candidates">
      <button
        type="button"
        class="inline-flex items-center justify-center gap-2 px-4 py-3 -mt-px -ml-px text-sm font-medium text-gray-700 align-middle transition-all bg-white border first:rounded-t-lg last:rounded-b-lg sm:first:rounded-l-lg sm:mt-0 sm:first:ml-0 sm:first:rounded-tr-none sm:last:rounded-bl-none sm:last:rounded-r-lg hover:bg-gray-50 focus:z-10 focus:outline-none focus:ring-2 focus:ring-blue-600 dark:bg-gray-800 dark:hover:bg-slate-800 dark:border-gray-700 dark:text-gray-400"
      >
        Find candidates
      </button>
    </RouterLink>
  </div>
</template>
