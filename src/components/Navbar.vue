<template>
  <div class="navbar h-28">
    <nav class="h-full flex flex-col ml-5 text-base leading-8 mb-4">
      <div class="flex h-20 items-center justify-between">
        <div class="flex items-center">
          <img class="rounded-md border p-1.5 grey" src="@/assets/burger.png" alt="Vector Image" />
          <img class="rounded-full h-8 ml-4" src="@/assets/github.png" alt="Vector Image" />
          <p class="font-semibold ml-3">Fabienmcll</p>
        </div>

        <div class="flex items-center space-x-3 mt-2">
          <div class="relative inline-flex items-center">
            <box-icon name="search" color="#969696" class="absolute left-2 h-5"></box-icon>
            <input class="bg-transparent border border-1 rounded p-1.5 h-7 pl-10 w-60" type="text" placeholder="Type / to search"/>
          </div>
          <div class="w-px h-5 trait"></div>

          <div class="border rounded flex items-center grey">
            <img class="p-1.5 grey" src="/src/assets/add.png" alt="Vector Image" />
            <img class="p-1.5 grey" src="/src/assets/down.png" alt="Vector Image" />
          </div>
          <div class="border rounded grey">
            <img class="p-1.5 grey" src="/src/assets/issues.png" alt="Vector Image" />
          </div>
          <div class="border rounded grey">
            <img class="p-1.5 grey" src="/src/assets/git.png" alt="Vector Image" />
          </div>
          <div class="border rounded grey">
            <img class="p-1.5 grey" src="/src/assets/notifications.png" alt="Vector Image" />
          </div>
          <div>
            <img class="grey border rounded-full grey mr-6" src="/src/assets/logos.png" alt="Vector Image" />
          </div>
        </div>
      </div>

      <ul class="flex p-2.5 mt-auto">
        <li class="ml-6 flex items-center nav-item" :class="{ 'active': $route.path === '/' }">
          <img class="h-4" src="@/assets/overview.png" />
          <router-link :to="'/'" class="ml-1 nav-link">Overview</router-link>
        </li>
        <li class="ml-6 flex items-center nav-item" :class="{ 'active': $route.path === '/repositories' }">
          <img class="h-4" src="@/assets/repositories.png" />
          <router-link :to="'#'" class="ml-1 nav-link">Repositories</router-link>
        </li>
        <li class="ml-6 flex items-center nav-item" :class="{ 'active': $route.path === '/projects' }">
          <img class="h-4" src="@/assets/projects.png" />
          <router-link :to="'#'" class="ml-1 nav-link">Projects</router-link>
        </li>
        <li class="ml-6 flex items-center nav-item" :class="{ 'active': $route.path === '/packages' }">
          <img class="h-4" src="@/assets/packages.png" />
          <router-link :to="'#'" class="ml-1 nav-link">Packages</router-link>
        </li>
        <li class="ml-6 flex items-center nav-item" :class="{ 'active': $route.path === '/stars' }">
          <img class="h-4" src="@/assets/stars.png" />
          <router-link :to="'#'" class="ml-1 nav-link">Stars</router-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
};
</script>

<style>
body {
  font-family: "Noto Sans", sans-serif;
}

.navbar {
  background-color: #010409;
  box-shadow: 0 0.5px 0 0 #9198a1;
}

.grey {
  border-color: #9198a1;
}

input {
  border-color: #9198a1;
}

.trait {
  background-color: #9198a1;
}

.nav-item {
  position: relative;
  display: flex;
  align-items: center;
}

.nav-item.active {
  font-weight: bold;
  color: #ffffff;
}

.nav-item.active::after {
  content: '';
  position: absolute;
  bottom: -3px;
  left: 0;
  width: 100%;
  height: 2px;
  background-color: #f78166;
  border-radius: 1px;
  box-shadow: 0 3px 5px rgba(247, 129, 102, 0.5);
}
</style>