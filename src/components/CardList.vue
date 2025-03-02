<script setup>
import Card from './Card.vue'

const onClickAdd = () => {
  alert('Added to cart')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      imageUrl="/sneakers/sneakers-1.jpg"
      name="Nike sneakers"
      :price="3000"
      :isFavorite="false"
      :isAdded="false"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
