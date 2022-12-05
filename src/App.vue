<script setup>
import { ref } from 'vue';

const to = ref(null);
const from = ref(null);
</script>
<template>
  <div class="w-full h-full flex justify-center items-center">
    <div>
      <div class="w-full max-w-2xl p-4 rounded bg-red-400 text-white">
        <div class="border-2 rounded flex flex-col md:flex-row md:items-center md:gap-8 p-4">
          <img src="/assets/santa.svg" alt="" class="max-w-[12em]" />
          <div>
            <h1 class="font-serif text-4xl">Happy Holidays!</h1>
            <div class="mt-4 bg-white text-black p-2 rounded">TO: {{ to }}</div>
            <div class="mt-2 bg-white text-black p-2 rounded">FROM: {{ from }}</div>
          </div>
        </div>
      </div>

      <div class="mt-8">
        <label class="block" for="to">
          To: <input type="text" id="to" v-model="to"
            class="rounded w-full border block  bg-gray-100 border-gray-300 focus:border-emerald-500 focus:ring-emerald-500 focus:ring p-1">
        </label>
      </div>
      <div class="mt-8">
        <label class="block" for="from">
          From: <input id="from" type="text" v-model="from"
            class="rounded w-full border block p-1  bg-gray-100 border-gray-300  focus:border-red-500 focus:ring-red-500 focus:ring">
        </label>
      </div>
    </div>


  </div>
</template>

