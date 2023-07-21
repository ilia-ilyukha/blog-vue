<script setup>
import { ref, reactive, computed } from 'vue';
import Post from './Post.vue'

const data = ref(null)
const posts = ref(null);
fetch("http://localhost:3002/posts")
    // .then(responce => console.log(responce))
    .then(responce => responce.json())
    .then(data => { 
        posts.value = data; 
        console.log(posts);
    });

</script>

<template>
    <div>
        <post v-for="post in posts" :key="post.id" :post="post">
        </post>
        
    </div>
</template>

<style></style>