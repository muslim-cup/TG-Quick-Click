<template>
  <section class="section-4">
    <div
      class="container bg-ms-color-10 py-[100px] flex gap-[30px] rounded-[30px]"
    >
      <div
        class="s4-blocks flex font-futur-regular items-start"
        v-for="item in options"
        :key="item.id"
      >
        <img :src="`/icons/${item.url}`" alt="" />
        <div class="s4-block-two px-[60px] w-[512px]">
          <h4 class="s4-h4 font-medium text-[40px]">
            {{ item.num }}
          </h4>
          <div class="s4-title font-medium text-[40px] mb-[50px] w-[100px]">
            {{ item.title }}
          </div>
          <div class="s4-text text-[20px] w-[454px]">{{ item.text }}</div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const options = [
  {
    url: "s4-logo1.png",
    num: "01",
    title: "Продуманный функционал",
    text: "Детально проработанный функционал с уникальной системой прокачки и продуманной реферальной системой",
  },
  {
    url: "s4-logo2.png",
    num: "02",
    title: "Гибкость модификаций",
    text: "Система разработанная максимально оптимизированным способом, позволяющим моментально и без проблем вносить любые модификации",
  },
];
</script>

<style>
</style>