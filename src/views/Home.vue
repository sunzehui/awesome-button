<script setup>
import CustomButton from '@/components/CustomButton.vue';

</script>

<template>
  <div class="bg-gray-50">
    <h2 class="text-center mt-5 text-2xl">Let's custom my button!</h2>
    <div class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8">
      <div class="px-4 py-6 sm:px-0">
        <div class="border-4 border-dashed border-gray-200 rounded-lg h-96">
          <div class="h-full grid grid-cols-3 grid-rows-1">
            <CustomButton />
            <div class="color-picker">
              <input type="color" id="head" name="head" value="#e66465">
              <input type="color" id="body" name="body" value="#f6f7eb">
              <input type="color" id="legs" name="legs" value="#f6f7eb">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
