<script setup>
const props = defineProps({
    post: Object
});
console.log(props);

</script>

<template>
    <article class="post">
        <header>
            <div class="title">
                <h2><a href="#">{{ post.title }}</a></h2>
                <p>{{ post.underTitle }}</p>
            </div>
            <div class="meta">
                <time class="published" datetime="{{ post.published.time }}">{{ post.published.time }}</time>
                <a href="#" class="author"><span class="name">{{ post.author.name }}</span><img
                        alt="" /></a>
                        
<!-- <a href="#" class="image featured"><img src="src/assets/images/pic01.jpg" alt="" /></a> -->
            </div>
        </header>
        <a href="#" class="image featured"><img src='{{ post.image }}' alt="" /></a>
        <p>{{ post.annotation }}</p>
        <footer>
            <ul class="actions">
                <li><a href="#" class="button big">Continue Reading</a></li>
            </ul>
            <ul class="stats">
                <li><a href="#">General</a></li>
                <li><a href="#" class="icon fa-heart">{{ post.hearts }}</a></li>
                <li><a href="#" class="icon fa-comment">{{ post.comments }}</a></li>
            </ul>
        </footer>
    </article>
</template>

<style></style>