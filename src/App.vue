<template>
  <div class="main">
    <post-form @create="createPost" />
    <post-list :posts="posts" />
  </div>
</template>

<script>
import PostForm from '@/components/PostForm.vue';
import PostList from '@/components/PostList.vue';
export default {
  data() {
    return {
      posts: [
        { id: 1, title: 'мыши', body: 'белые и черные' },
        { id: 2, title: 'кошки', body: 'белые и черные' },
        { id: 3, title: 'собаки', body: 'белые и черные' },
      ],
      title: '',
      body: '',
    };
  },
  components: { PostForm, PostList },
  methods: {
    createPost(post) {
      this.posts.push(post);
    },
    inputValue(e) {
      this.title = e.target.value;
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
</style>
