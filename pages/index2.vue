
<template>

<Center prop="タルコフ紹介"/>
<training/>
<div class="container text-center my-5">
<p>{{ index.syokai }}</p>
</div>
<div id= "App1">
    <li v-for="item in index.itemlist"
    :prop1="item">{{ item.text }}</li>
</div>

</template>
<script setup land="ts">

 './components/training.vue';
 './components/Center.vue'
 const index = Usetrukohu();
 definePageMeta({
  layout: 'custom'
})
</script>