.
<template>
  <div>
    <div class="px-4 sm:px-0">
      <h3 class="text-base font-semibold leading-7 text-gray-900">
        Applicant Information
      </h3>
      <p class="max-w-2xl mt-1 text-sm leading-6 text-gray-500">
        Personal details and application.
      </p>
    </div>
    <div class="mt-6 border-t border-gray-100">
      <dl class="divide-y divide-gray-100">
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">Full name</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">
            Margot Foster
          </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">Application for</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">
            Backend Developer
          </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">Email address</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">
            margotfoster@example.com
          </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">Salary expectation</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">
            $120,000
          </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">About</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">
            Fugiat ipsum ipsum deserunt culpa aute sint do nostrud anim incididunt cillum
            culpa consequat. Excepteur qui ipsum aliquip consequat sint. Sit id mollit
            nulla mollit nostrud in ea officia proident. Irure nostrud pariatur mollit ad
            adipisicing reprehenderit deserunt qui eu.
          </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900">Attachments</dt>
          <dd class="mt-2 text-sm text-gray-900 sm:col-span-2 sm:mt-0">
            <ul
              role="list"
              class="border border-gray-200 divide-y divide-gray-100 rounded-md"
            >
              <li
                class="flex items-center justify-between py-4 pl-4 pr-5 text-sm leading-6"
              >
                <div class="flex items-center flex-1 w-0">
                  <!-- <PaperClipIcon class="flex-shrink-0 w-5 h-5 text-gray-400" aria-hidden="true" /> -->
                  <div class="flex flex-1 min-w-0 gap-2 ml-4">
                    <span class="font-medium truncate"
                      >resume_back_end_developer.pdf</span
                    >
                    <span class="flex-shrink-0 text-gray-400">2.4mb</span>
                  </div>
                </div>
                <div class="flex-shrink-0 ml-4">
                  <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500"
                    >Download</a
                  >
                </div>
              </li>
              <li
                class="flex items-center justify-between py-4 pl-4 pr-5 text-sm leading-6"
              >
                <div class="flex items-center flex-1 w-0">
                  <!-- <PaperClipIcon class="flex-shrink-0 w-5 h-5 text-gray-400" aria-hidden="true" /> -->
                  <div class="flex flex-1 min-w-0 gap-2 ml-4">
                    <span class="font-medium truncate"
                      >coverletter_back_end_developer.pdf</span
                    >
                    <span class="flex-shrink-0 text-gray-400">4.5mb</span>
                  </div>
                </div>
                <div class="flex-shrink-0 ml-4">
                  <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500"
                    >Download</a
                  >
                </div>
              </li>
            </ul>
          </dd>
        </div>
      </dl>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from "vue";
import { useRoute } from "vue-router";

const route = useRoute();

onMounted(() => {
  const { person } = route.params
  console.log(JSON.parse(person));
});
</script>
