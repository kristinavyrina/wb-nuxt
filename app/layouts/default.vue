<template>
  <Header />

  <slot />

  <Footer />

  <Cart v-if="viewCart"/>
</template>
<script setup>
import {useViewCart} from "~/composables/states.js";

const viewCart = useViewCart()
</script>