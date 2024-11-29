<template>
  <div class="flex">
    <div class=" left h-[calc(100vh-135px)]">
      <div class="h-80 flex justify-end">
        <img class="border border-gray-600 rounded-full h-68 mr-6 mt-10" src="@/assets/logo_fabien.jpeg">
      </div>
      <div class="flex flex-wrap w-full mt-4">
        <div class="width "></div>
        <div class="w-2/5">
          <p class="font-semibold text-2xl">Fabien</p>
          <p class="font-normal text-xl	text-gray-500">Fabienmcll</p>
          <button class="border border-gray-600 rounded w-full bg-[#262C36] py-0.5 mt-4 ">Follow</button>
          <p class="mt-4">Hello World !</p>
          <div class="flex items-center mt-4">
            <img class="h-5" src="@/assets/follow.png" alt="Logo">
            <p class="text-sm ml-2">
              7 <span class="text-gray-500">Followers</span> •
              13 <span class="text-gray-500">Following</span>
            </p>
          </div>
          <div class="text-sm flex flex-col items-start mt-5">
            <div class="flex items-center">
              <img class="h-5 mr-2" src="@/assets/formation.png" alt="Formation">
              <p>CFAI LDA : BAC + 3 CPLR</p>
            </div>
            <div class="flex items-center mt-3">
              <img class="h-5 mr-2" src="@/assets/map.png" alt="Location">
              <p>Saint Etienne, France</p>
            </div>
            <div class="flex items-center mt-3">
              <img class="h-5 mr-2" src="@/assets/link.png" alt="Location">
              <a class="hover:text-blue-500" target="_blank" href="http://fabienmcl.fr">fabienmcl.fr</a>
            </div>
            <div class="flex items-center mt-3">
              <img class="h-5 mr-2" src="@/assets/link.png" alt="Location">
              <a class="hover:text-blue-500" target="_blank" href="http://gitea.fabienmcl.fr/fabienmcll">gitea.fabienmcl.fr</a>
            </div>
            <hr class="border-t border-gray-600 w-full mt-4">
          </div>
          <div class="mt-4">
            <p class="font-semibold	">Achievements</p>
            <img class="h-14 mt-2" src="@/assets/shark.png">
          </div>
        </div>
      </div>
    </div>
    </div>
</template>

<style>
.left {
  width: 35%;
}

.width{
  width: 55%;
}
</style>

<script>
export default {
  name: 'Profil',
};
</script>
