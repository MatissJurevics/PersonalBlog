<script setup>
import { computed, ref } from "vue";
import PostCard from "../components/PostCard.vue";
const posts = ref(["Title1", "Title2", "Title3", "Title4", "Title5", "Title6"]);
// Token 1a3e2b3b2a638dd5ffc748d271c02c3a8b2a1cc6a5f225227d027fdbef7c3547aa6e8b3760e9ebd47d9173f09493cb78412145436125085ed1968637c72b2a6a21fecbafab5df5e34f01390235a457402aceae52531c9cb9f193f3fe4d6c706d2df454063d6c8ddd95077912c8b5764b3e46c38bdc770aea88850883538cf47a

</script>

<template>
  <main>
    <header
      class="min-h-[60vh] w-full bg-base-200 flex flex-col items-center justify-center"
    >
      <div
        class="w-full flex flex-col lg:flex-row items-center justify-around px-64"
      >
        <img
          src="https://placeimg.com/600/400/arch"
          alt=""
          class="max-h-md max-w-xl rounded-lg"
        />
        <div class="max-w-xl h-md flex flex-col justify-around text-right">
          <h1 class="text-4xl font-bold">This is a sample Blog post!</h1>
          <p class="font-light text-lg">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Neque,
            soluta voluptate corrupti omnis quos accusantium non quia nisi
            delectus excepturi....
          </p>
          <nuxt-link
            class="btn btn-primary max-w-[150px] xl:ml-auto hover:shadow-md hover:shadow-primary"
            to="/"
            >Read Now!</nuxt-link
          >
        </div>
      </div>
    </header>

    <section class="w-full px-32 py-16">
      <h1 class="text-content text-3xl font-semibold">Blog Posts</h1>
      <ul class="flex flex-col xl:flex-row  flex-wrap">
        <PostCard v-for="post in posts" :title="post"/>

       
      </ul>
    </section>
  </main>
</template>
