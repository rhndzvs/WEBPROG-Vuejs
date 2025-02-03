<template>
  <div class="comments-container">
    <h1>Comments</h1>
    <ul>
      <li v-for="comment in comments" :key="comment.id" class="comment-item">
        <div class="comment-name">{{ comment.name }}</div>
        <div class="comment-text">{{ comment.comment }}</div>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import { supabase } from '../lib/supabaseClient';

const comments = ref([]);

async function getComments() {
  const { data, error } = await supabase.from('comments').select();
  if (error) {
    console.error("Error fetching comments:", error);
  } else {
    comments.value = data;
  }
}

onMounted(() => {
  getComments();
});
</script>

<style scoped>
.comments-container {
  border: dashed black 1px;
  display: inline-block;
  margin: 10px;
  padding: 10px;
  background-color: lightyellow;
  width: 100%;
  max-width: 600px;
}

.comment-item {
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-gap: 10px;
  margin-bottom: 10px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

.comment-name {
  font-weight: bold;
}

.comment-text {
  word-wrap: break-word;
}
</style>