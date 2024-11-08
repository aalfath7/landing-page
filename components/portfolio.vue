<template>
  <section id="portfolio" class="py-36">
    <h2 class="text-end text-3xl sm:text-4xl relative">
      <span class="absolute top-0 -translate-x-10 -translate-y-3">__</span>
      Portfolio
    </h2>
    <div class="grid sm:grid-cols-3 gap-20 py-10">
      <div
        v-for="item in data"
        class="bg-white border border-gray-200 shadow dark:bg-gray-800 dark:border-gray-700"
      >
        <a href="#">
          <img class="rounded-t-lg" :src="item.img" alt="" />
        </a>
        <div class="p-5">
          <a href="#">
            <h5
              class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
            >
              {{ item.title }}
            </h5>
          </a>
          <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
            {{ item.desc }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const data = [
  {
    title: "EduTajwid",
    desc: "An interactive Tajweed learning website. A Tajweed learning website for children, teenagers, and adults with engaging lessons.",
    img: "/project-1.png",
  },
  {
    title: "EduTajwid",
    desc: "An interactive Tajweed learning website. A Tajweed learning website for children, teenagers, and adults with engaging lessons.",
    img: "/project-1.png",
  },
  {
    title: "EduTajwid",
    desc: "An interactive Tajweed learning website. A Tajweed learning website for children, teenagers, and adults with engaging lessons.",
    img: "/project-1.png",
  },
];
</script>
