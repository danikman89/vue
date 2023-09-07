<template>
  <div class="main">
    <form>
      <h4>Создание поста</h4>
      <input class="input" type="text" placeholder="Название" />
      <input class="input" type="text" placeholder="Описание" />
      <button class="btn">Создать</button>
    </form>
    <div v-for="post in posts" class="post">
      <div><strong>Название:</strong> {{ post.title }}</div>
      <div><strong>Описание:</strong> {{ post.body }}</div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        { id: 1, title: 'мыши', body: 'белые и черные' },
        { id: 2, title: 'кошки', body: 'белые и черные' },
        { id: 3, title: 'собаки', body: 'белые и черные' },
      ],
    };
  },
  methods: {
    addLike() {
      this.likes += 1;
    },
    addDislike() {
      this.dislikes += 1;
    },
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main {
  padding: 20px;
}

.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}

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
