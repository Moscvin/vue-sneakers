<script setup>
import DrawerHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>
<template>
  <div>
    <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-50"></div>
    <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
      <DrawerHead />
      <CartItemList />
      <div>
        <div class="flex gap-4">
          <span>total:</span>
          <div class="flex-1 border-b border-dashed"></div>
          <b>300 $</b>
        </div>
        <div class="flex gap-2">
          <span>Impozit 5% :</span>
          <div class="flex-1 border-b border-dashed"></div>
          <b>15 $</b>
        </div>
      </div>
      <button class="bg-lime-400 w-full rounded-xl py-3 transition duration-1000 hover:bg-blue-500">
        Save
      </button>
    </div>
  </div>
</template>
