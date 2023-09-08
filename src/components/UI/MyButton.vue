<template>
  <button>
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
  margin-top: 15px;
  cursor: pointer;
}
</style>
