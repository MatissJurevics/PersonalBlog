<template>
  <main class="w-screen min-h-screen bg-base-100 lg:px-32">
    <header
      class="min-h-[65vh] my-8 rounded-xl bg-neutral flex flex-row justify-center items-center"
    >
      <h1 class="text-4xl font-extrabold text-white tracking-tight">
        Welcome to my Blog
      </h1>
    </header>

    <section class="flex flex-col lg:flex-row px-40">
      <div
        class="min-h-[24rem] lg:w-1/2 bg-neutral p-6 rounded-xl my-8 lg:mr-4"
      >
        <h2 class="text-3xl text-white font-bold mb-4">About Me 👋</h2>
        <p class="text-xl font-light">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum
          quidem voluptates nihil incidunt iure repellat expedita perferendis
          velit, pariatur a tempore, commodi hic recusandae doloribus in nobis
          reiciendis asperiores vero.
        </p>
      </div>
      <div class="my-8 flex flex-col justify-between lg:w-1/2 lg:ml-4">
        <Article />
        <div class="min-h-[12rem] w-full bg-neutral rounded-xl mt-4 p-4">
          <div>
            <h2 class="text-2xl text-white font-bold mb-4">Find Me On</h2>
            <div>
              <a href="#">Twitter</a>
              <a href="#">Github</a>
              <a href="#">LinkedIn</a>
            </div>
          </div>

          <span class="font-semibold">
            Send me an email at 
            <b>matissjurevics@gmail.com</b>
          </span>
        </div>
      </div>
    </section>
    <section class="px-40">
        <h1 class="text-3xl font-bold text-white mt-4">Newest Posts</h1>
        <div>
            
        </div>
    </section>
  </main>
</template>
