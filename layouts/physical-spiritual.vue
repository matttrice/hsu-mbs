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
    <div :class='props.class' class='center-bleed' >
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