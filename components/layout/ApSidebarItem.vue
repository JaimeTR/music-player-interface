<template>
  <div
    :class="[{ 'text-yellow-500': active }]"
    class="
      w-full
      relative
      cursor-pointer
      group
      py-1
      mt-2
      font-inter
      hover:text-yellow-500
      text-gray-700
      font-medium
      text-sm
      select-none
    "
  >
    <slot />
    <div
      :class="[{ 'bg-yellow-500': active }]"
      class="
        identifier
        w-1
        h-full
        absolute
        right-0
        top-0
        transition-all
        duration-200
      "
    ></div>
  </div>
</template>

<script>
export default {
  name: 'ApSidebarItem',
  props: {
    active: { type: Boolean, default: false },
  },
}
</script>
