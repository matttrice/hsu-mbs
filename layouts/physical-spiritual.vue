<!--
  Usage:
```md
---
layout: physical-spiritual
---
::left::
This shows on the left

::physical:: 
This shows left center in gray

::middle::
Center of page

::spiritual::
This shows right center in blue

::right::
This shows on the right
```
-->

<script setup lang='ts'>
const props = defineProps({
  class: {
    type: String,
  },
})
</script>

<template>
  <div class='grid grid-cols-[1fr_1fr_5px_1fr_1fr]'>

    <!--------------left------------------->
    <div class='text-2xl' :class='props.class'>
      <slot name='left' />
    </div>

    <!--------------spiritual------------------->
    <div class='bg-sky-400
                      text-blue-800
                      brick-head' :class='props.class'>
      <slot name='spiritual' />
    </div>

    <!--------------middle------------------->
    <div :class='props.class'>
      <slot name='middle' />
    </div>

    <!--------------physical------------------->
    <div class='bg-gray-400
                      text-zinc-800
                      brick-head' :class='props.class'>
      <slot name='physical' />
    </div>

    <!--------------right------------------->
    <div class='text-2xl' :class='props.class'>
      <slot name='right' />
    </div>
  </div>
</template>

<style>
.brick-head {
  @apply text-3xl border-black [&>*:first-child]:text-5xl [&>*:first-child]:border-b-2 [&>*:first-child]:border-black [&>*:first-child]:font-bold
}

.brick {
  @apply bg-white p-b-28 p-t-1 absolute w-full m-b-15 z-1
}

.sidebox {
  @apply rounded-lg p-2 m-t-3 bg-white text-base w-1/2 text-blue-700;
}
</style>