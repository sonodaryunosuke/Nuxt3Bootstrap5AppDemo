<template>

<Center prop="タルコフ紹介"/>
<training/>
<div class="container text-center my-5">
<p>{{ index.syokai }}</p>
</div>
<li v-for="item in index.material">{{ item.text }}</li>
<a href = "index2">こちら</a>
</template>
<script setup land="ts">
 './components/training.vue';
 './components/Center.vue'
 const index = Usetrukohu();
 definePageMeta({
  layout: 'default'
})
</script>
