<template>
  <button>like</button>
  <button>dislike</button>
  <div>
    Кол-во лайков: <strong>{{ likes }}</strong>
  </div>
  <div>
    Кол-во дизлайков: <strong>{{ dislikes }}</strong>
  </div>
</template>

<script>
export default {
  data() {
    return {
      likes: 0,
      dislikes: 0,
    };
  },
};
</script>

<style scoped></style>
