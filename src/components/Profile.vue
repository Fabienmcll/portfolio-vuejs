<template>
  <div class="flex">
    <div class=" left h-[calc(100vh-135px)]">
      <div class="h-80 flex justify-end">
        <img class="border rounded-full h-68 mr-6 mt-10" src="@/assets/logo_fabien.jpeg">
      </div>
      <div class="flex flex-wrap w-full mt-4">
        <div class="width "></div>
        <div class="w-2/5">
          <p class="font-semibold text-xl	">Fabien</p>
          <p class="font-normal text-xl	text-gray-500">Fabienmcll</p>
          <button class="border rounded w-full bg-gray-800 py-0.5 mt-4 ">Follow</button>
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
