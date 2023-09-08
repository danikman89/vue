<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {};
</script>

<style scoped>
.btn {
  background: none;
  padding: 10px 20px;
  color: teal;
  border: 1px solid teal;
  cursor: pointer;
}
</style>
