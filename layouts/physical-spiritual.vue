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
  <div  bg-slate-300 class='grid grid-cols-[1fr_1fr_5px_1fr_1fr]'>

    <!--------------left------------------->
    <div class='text-2xl txt-carnal' :class='props.class'>
      <slot name='left' />
    </div>

    <!--------------spiritual------------------->
    <div class='bg-spirit txt-spirit' :class='props.class'>
      <slot name='spiritual' />
    </div>

    <!--------------middle------------------->
    <div :class='props.class' bg-black z-1 p='relative'>
      <slot name='middle' />
    </div>

    <!--------------physical------------------->
    <div class='bg-carnal txt-carnal' :class='props.class'>
      <slot name='physical' />
    </div>

    <!--------------right------------------->
    <div class='text-2xl txt-carnal' :class='props.class'>
      <slot name='right' />
    </div>
  </div>
</template>