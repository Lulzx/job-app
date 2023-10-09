<template>
    <div class="flex items-center justify-between px-4 py-3 bg-white border-t border-gray-200 sm:px-6">
      <ul class="space-y-4">
      <li v-for="item in items" :key="item.id" class="p-4 transition-colors duration-300 bg-white hover:bg-gray-100">
        <div class="text-lg font-semibold">{{ item.title }}</div>
        <div class="text-gray-500">{{ item.department }}</div>
        <div class="text-gray-500">{{ item.type }}</div>
        <div class="text-gray-500">{{ item.location }}</div>
      </li>
    </ul>
    </div>
  </template>

  <script setup>
  // import { ChevronLeftIcon, ChevronRightIcon } from '@heroicons/vue/20/solid'

  const items = [
    { id: 1, title: 'Back End Developer', department: 'Engineering', type: 'Full-time', location: 'Remote' },
    { id: 2, title: 'Front End Developer', department: 'Engineering', type: 'Full-time', location: 'Remote' },
    { id: 3, title: 'User Interface Designer', department: 'Design', type: 'Full-time', location: 'Remote' },
  ]
  </script>