<template>
  <Jumbotron />
  <div class="px-5 sm:px-36 py-5 space-y-10">
    <About />
    <Portfolio />
    <Contact />
  </div>
</template>

<script setup>
useHead({
  title: "fath | All About Me",
  meta: [{ name: "frontend developer", content: "My amazing site." }],
});

import AOS from "aos";
import "aos/dist/aos.css";

onMounted(() => {
  AOS.init();
});
</script>
