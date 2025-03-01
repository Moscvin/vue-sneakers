<script setup>
const props = defineProps({
  title: String,
  price: Number,
  isAdded: Boolean,
})
console.log(props)
</script>

<template>
  <div class="product">
    <h2>sneaker:{{ title }}</h2>
    <h3>price:{{ price }}</h3>
    <h4>Added :{{ isAdded }}</h4>
    <slot></slot>
  </div>
</template>
<style>
.product {
  border: 1px blue solid;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
