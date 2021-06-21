<template>
  <section class="pl-6 py-6">
    <p
      class="uppercase font-inter text-gray-400 font-medium text-sm select-none"
    >
      {{ title }}
    </p>
    <slot />
  </section>
</template>

<script>
export default {
  name: 'GroupSidebar',
  props: {
    title: { type: String, default: '' },
  },
}
</script>
