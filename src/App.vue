<template>
  <div>
    <div class="post">
      <div><strong>Название:</strong> пост о мышах и людях</div>
      <div><strong>Описание:</strong> мыши белые и пушичтые</div>
    </div>
    <div class="post">
      <div><strong>Название:</strong> пост о мышах и людях</div>
      <div><strong>Описание:</strong> мыши белые и пушичтые</div>
    </div>
    <div class="post">
      <div><strong>Название:</strong> пост о мышах и людях</div>
      <div><strong>Описание:</strong> мыши белые и пушичтые</div>
    </div>
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

.post {
  padding: 15px;
  border: 2px solid teal;
  margin-top: 15px;
}
</style>
