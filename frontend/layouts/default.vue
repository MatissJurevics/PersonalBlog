<template>
  <div class="drawer" data-theme="night">
    <input id="my-drawer-3" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content flex flex-col ">


      <!-- Navbar -->
      <nav class="w-full navbar bg-base-300">
        <div class="flex-none lg:hidden">
          <label for="my-drawer-3" class="btn btn-square btn-ghost">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              class="inline-block w-6 h-6 stroke-current"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              ></path>
            </svg>
          </label>
        </div>
        <div class="flex-1 px-2 mx-2 text-xl">Blog</div>
        <nav class="flex-none hidden lg:block">
          <ul class="menu menu-horizontal">
            <!-- Navbar menu content here -->
            <li class="rounded-xl"><a>Portfolio</a></li>
            <li class="rounded-xl"><a>IDK</a></li>
          </ul>
        </nav>
      </nav>
      <!-- Page content here -->

      <main class="max-w-screen h-auto">
        <slot />
      </main>

      <footer class="footer footer-center p-4 bg-base-300 text-base-content mt-auto">
        <div>
          <p>Made by: <a class="font-bold hover:scale-110" href="https://www.saetom.xyz">Matiss Jurevics</a> (2022)</p>
        </div>
      </footer>


    </div>
    <div class="drawer-side">
      <label for="my-drawer-3" class="drawer-overlay"></label>
      <ul class="menu p-4 overflow-y-auto w-80 bg-base-100">
        <!-- Sidebar content here -->
        <li><a>Sidebar Item 1</a></li>
        <li><a>Sidebar Item 2</a></li>
      </ul>
    </div>
  </div>
</template>
