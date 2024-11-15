<template>
  <section id="portfolio" class="py-36 px-5">
    <h2 class="text-end text-3xl sm:text-4xl relative text-white">
      <span class="text-white absolute top-0 -translate-x-10 -translate-y-3"
        >__</span
      >
      Portfolio
    </h2>
    <div class="grid sm:grid-cols-3 gap-20 py-10">
      <div
        v-for="(item, index) in data"
        data-aos="fade-down"
        :data-aos-delay="index * 50 + 50"
        class="bg-white border border-gray-200 shadow"
      >
        <a :href="item.link" target="_blank">
          <img class="rounded-t-lg" :src="item.img" alt="" />
        </a>
        <div class="p-5">
          <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900">
              {{ item.title }}
            </h5>
          </a>
          <p
            class="mb-3 font-normal text-gray-600 dark:text-gray-400 line-clamp-3"
          >
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
    title: "edutajwid.com",
    desc: "An interactive Tajweed learning website. A Tajweed learning website for children, teenagers, and adults with engaging lessons.",
    img: "/edutajwid.png",
    link: "https://edutajwid.com",
  },
  {
    title: "auladianaindonesia.sch.id",
    desc: "A school profile website showcasing the school's profile, news, registration features, and additional sections such as academic programs, student achievements, and contact information.",
    img: "/auladina.png",
    link: "https://auladinaindonesia.sch.id",
  },
  {
    title: "racikalcencekia.sch.id",
    desc: "Cikal Cendekia Islamic School is an Islamic Fullday School that integrates the National Curriculum with Islamic values, focusing on developing students' noble character and integrity. The school offers a Qur'an memorization program and various extracurricular activities, such as drumband and calligraphy, to support students' talent development.",
    img: "/racikal.png",
    link: "https://racikalcendekia.sch.id",
  },
];
</script>
