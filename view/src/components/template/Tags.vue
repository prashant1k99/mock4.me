<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <span
    class="inline-flex items-center bg-gray-100 px-2.5 py-0.5 font-medium text-gray-800" 
    :class="[rounded ? 'rounded-full': 'rounded-md', large? 'text-sm' : 'text-xs']" 
    v-bind="$attrs">
    <slot></slot>
  </span>
</template>

<script>
export default {
  props: {
    large: Boolean,
    rounded: Boolean
  }
}
</script>