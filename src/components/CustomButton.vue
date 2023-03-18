<script setup>
const props = defineProps({
  // Define props here
  bgColor: {
    type: String,
    default: '#ffffff'
  },
  textColor: {
    type: String,
    default: '#000000'
  },
  borderColor: {
    type: String,
    default: '#000000'
  },
  hoverBgColor: {
    type: String,
    default: '#ffffff'
  },
  hoverTextColor: {
    type: String,
    default: '#000000'
  },
  hoverBorderColor: {
    type: String,
    default: '#000000'
  },
  focusBgColor: {
    type: String,
    default: '#ffffff'
  },
  focusTextColor: {
    type: String,
    default: '#000000'
  },
  focusBorderColor: {
    type: String,
    default: '#000000'
  },
})
const _style = {
  backgroundColor: props.bgColor,
  color: props.textColor,
  borderColor: props.borderColor,
  hoverBgColor: props.hoverBgColor,
  hoverTextColor: props.hoverTextColor,
  hoverBorderColor: props.hoverBorderColor,
  focusBgColor: props.focusBgColor,
  focusTextColor: props.focusTextColor,
  focusBorderColor: props.focusBorderColor,
}
</script>
<template>
  <div class="button-item h-full w-full flex flex-col items-center justify-center">
    <button
      class="shadow inline-flex items-center justify-center px-8 py-3 text-base font-medium leading-6 transition duration-150 ease-in-out bg-white border border-transparent rounded-md focus:outline-none custom-btn">
      Button
    </button>
  </div>
</template>

<style lang="scss">
.custom-btn {
  background-color: bind('_style.bgColor');
  color: bind('_style.textColor');
  border-color: bind('_style.borderColor');

  &:hover {
    background-color: bind('_style.hoverBgColor');
    color: bind('_style.hoverTextColor');
    border-color: bind('_style.hoverBorderColor');
  }

  &:focus {
    background-color: bind('_style.focusBgColor');
    color: bind('_style.focusTextColor');
    border-color: bind('_style.focusBorderColor');
  }

}
</style>
