<template>
  <div
    class="md:w-1/3 w-full p-4 pb-6 max-md:mb-4 hover:bg-blue-700 hover:text-white transition-all ease duration-300 bg-white shadow rounded group"
  >
    <div class="flex gap-x-4">
      <div class="w-14 h-14 bg-white p-2 rounded">
        <slot />
      </div>
      <div>
        <p class="text-xl font-semibold">{{ judul }}</p>
        <p class="font-light text-slate-400 group-hover:text-slate-200">
          {{ tech }}
        </p>
      </div>
    </div>
    <div class="my-4 mb-12">
      <p class="text-slate-600 group-hover:text-slate-100">
        {{ deskripsi }}
      </p>
    </div>
    <div class="flex justify-between items-center">
      <div>
        <button
          type="button"
          class="bg-slate-200 px-4 py-1 rounded-full group-hover:bg-blue-600 group-hover:text-white font-semibold"
        >
          {{ lang }}
        </button>
      </div>
      <div>
        <p class="font-semibold">{{ gaji }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  judul: String,
  tech: String,
  deskripsi: String,
  lang: String,
  gaji: String,
});
// export default {
//   props: ["judul", "tech", "deskripsi", "lang", "gaji"],
// };
</script>
