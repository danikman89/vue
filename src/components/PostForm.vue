<template>
  <form @submit.prevent>
    <h4>Создание поста</h4>
    <input
      v-bind:value="title"
      @input="inputValue"
      class="input"
      type="text"
      placeholder="Название"
    />
    <input
      v-bind:value="body"
      @input="body = $event.target.value"
      class="input"
      type="text"
      placeholder="Описание"
    />
    <button class="btn" @click="createPost">Создать</button>
  </form>
</template>

<script>
export default {};
</script>

<style scoped>
form {
  display: flex;
  flex-direction: column;
}

.input {
  width: 100%;
  border: 1px solid teal;
  padding: 15px;
  margin-top: 15px;
}

.btn {
  background: none;
  padding: 10px 20px;
  color: teal;
  align-self: flex-end;
  border: 1px solid teal;
  margin-top: 15px;
  cursor: pointer;
}

.btn:hover {
  color: white;
  background-color: teal;
}
</style>
