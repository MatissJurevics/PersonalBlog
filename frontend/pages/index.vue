<template>
  <header
    class="min-h-[60vh] w-full bg-base-200 flex flex-col items-center justify-center"
  >
    <div class="w-full flex flex-col lg:flex-row items-center justify-around">
      <img
        src="https://placeimg.com/600/400/arch"
        alt=""
        class="max-h-md max-w-xl rounded-lg"
      />
      <div class="max-w-xl h-full flex flex-col justify-around text-right">
        <h1 class="text-4xl font-bold">This is a sample Blog post!</h1>
        <p class="font-light text-lg">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Neque,
          soluta voluptate corrupti omnis quos accusantium non quia nisi
          delectus excepturi....
        </p>
        <nuxt-link class="btn btn-primary max-w-[150px] xl:ml-auto hover:shadow-md hover:shadow-primary" to="/"
          >Read Now!</nuxt-link
        >
      </div>
    </div>
  </header>
</template>
