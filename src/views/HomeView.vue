<script setup lang="ts">
import IconLight from '@/components/icons/IconLight.vue'
import IconNotifications from '@/components/icons/IconNotifications.vue'
import IconSetting from '@/components/icons/IconSetting.vue'
import IconSquare from '@/components/icons/IconSquare.vue'
import IconCloud from '@/components/icons/IconCloud.vue'
</script>

<template>
  <main class="h-screen w-full flex justify-start items-center px-10">
    <div class="flex w-full relative gap-10">
      <section>
        <ul class="py-10 px-2 text-gray-100 group bg-black/10 backdrop-blur-md flex flex-col gap-4 ul rounded-full">
          <li class="cursor-pointer  p-4 text-2xl transition rounded-full hover:bg-white/50">
            <IconSquare class="group-hover:text-white" />
          </li>
          <li class="cursor-pointer group p-4 text-2xl transition rounded-full hover:bg-white/50">
            <IconLight class="group-hover:text-white" />
          </li>
          <li class="cursor-pointer group p-4 text-2xl transition rounded-full hover:bg-white/50">
            <IconNotifications class="group-hover:text-white" />
          </li>
          <li class="cursor-pointer group p-4 text-2xl transition rounded-full hover:bg-white/50">
            <IconSetting class="group-hover:text-white"/>
          </li>
        </ul>
      </section>
      <section class="relative flex w-full ">
        <div class="p-7 w-1/4 rounded-xl  aside h-full bg-black/10 backdrop-blur-md">
          <div class="bg-white/60 p-5 backdrop-blur-sm rounded-xl">
            <h3 class="text-xl text-white font-medium">Temperature outside</h3>
            <div class="flex gap-10 mt-5 items-center  ">
              <div class="relative">
                <div 
                  class="
                    absolute w-14 h-14 bg-gradient-to-t from-[#f07706] 
                    to-[#ffca99] rounded-full top-2 -right-5 z-0 soleil
                  "
                >
                </div>
                <IconCloud class="w-16 text-white h-16 z-10 relative"/>
              </div>
              <div class="">
                <h3 class="text-5xl font-bold text-white">26°C</h3>
                <p class="text-white text-lg">Lubumbashi, DRC</p>
              </div>
            </div>
          </div>
        </div>
        <div class="p-5 w-8/12">

        </div>
      </section>
    </div>
  </main>
</template>
<style scoped>
main{
  background: url('https://media.istockphoto.com/id/1408400512/photo/creative-composition-of-home-garden-interior-filled-a-lot-of-beautiful-plants-cacti.webp?s=2048x2048&w=is&k=20&c=9EntY1ueQfzLWo_EJhLOGn6kElhsPpx4_ZXIVqb0qWk=');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
.ul{
  box-shadow: inset 1px 1px 0.12px rgba(255, 255, 255, 0.651),
  1px 1px 3px rgba(0, 0, 0, 0.1);

}
.aside{
  box-shadow: inset 0px 1px 0.12px rgba(255, 255, 255, 0.651),
  1px 1px 3px rgba(0, 0, 0, 0.1);

}
.soleil{
  -webkit-box-shadow: 4px -9px 300px 200px rgb(230, 142, 61);
  -moz-box-shadow: 4px -9px 300px 200px rgba(230, 142, 61);
  box-shadow: 3px 7px 20px 5px rgba(230, 142, 61);
}
.cloud{
  z-index: 9 !important;
}
</style>