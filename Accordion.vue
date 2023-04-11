<script setup>
import { ref } from "vue";
const isOpen = ref(false);
</script>
<template>
    <div class="">
      <div class="px-4 py-5 sm:p-6">
        <h3 class="text-base font-semibold leading-6 text-gray-900 cursor-pointer" @click="isOpen = !isOpen">Manage subscription</h3>
        <div :class="isOpen ? 'd-block' : 'hidden'">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reprehenderit enim nobis vero amet, debitis expedita dolore minima distinctio cumque eum.</p>
        </div>
      </div>
    </div>
</template>
  
