<script setup>
import { defineProps } from 'vue';

const props = defineProps({
      text: {
            type: Array,
            required: true
      }
});
</script>

<template>
      <div class="flex gap-2 text-sm">
            <div v-for="(langItem, index) in text" :key="index" class=" border border-white bg-inherit rounded-full py-2 px-3">
                  {{ langItem.text }}
            </div>
      </div>
</template>

<style scoped>

</style>