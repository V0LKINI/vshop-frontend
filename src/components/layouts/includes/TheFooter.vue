<template>
  <div class="w-full ">
    <ul>
      <li v-for="link in links" :key="link.id">
        <router-link :to="link.href">
          {{ link.name }}
        </router-link>
      </li>
    </ul>
  </div>
</template>


<script setup>
const links = [
  {id: 1, name: 'Главная', href: '/'},
  {id: 2, name: 'Каталог', href: '/catalog/'},
];
</script>


