<script setup>
import { computed, ref } from "vue";
const posts = ref(["Title1", "Title2", "Title3", "Title4", "Title5", "Title6"]);
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
      <ul class="flex flex-col xl:flex-row flex-wrap">
        <div v-for="post in posts" class="card w-96 bg-base-100 shadow-xl mr-8 my-8">
          <figure>
            <img src="https://placeimg.com/400/225/arch" alt="Shoes" />
          </figure>
          <div class="card-body">
            <h2 class="card-title">
              {{post}}
              <div class="badge badge-secondary">NEW</div>
            </h2>
            <p>If a dog chews shoes whose shoes does he choose?</p>
            <div class="card-actions justify-end">
              <div class="badge badge-outline">Fashion</div>
              <div class="badge badge-outline">Products</div>
            </div>
          </div>
        </div>
      </ul>
    </section>
  </main>
</template>
