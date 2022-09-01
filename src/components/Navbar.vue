<template>
  <div class="fixed flex w-full z-40 top-0 lg:bg-gradient-to-r from-black to-black2 lg:h-20 sm:bg-black sm:h-16 ">
    <div class="flex font-serif flex-row w-full h-full justify-between items-center sm:px-8 lg:px-0">

      <!--hamburger menu-->
      <button class="focus:outline-none text-blue-500 items-center lg:hidden sm:flex ">
          <span class="material-icons text-3xl">
          menu
          </span>
        </button>
      <!--end-->

      <div class="flex flex-row space-x-8 text-white h-full">
        <button class="focus:outline-none flex items-center lg:ml-12">
          <img src="../assets/imgs/navAion.png" class="lg:w-36 sm:w-24"/>
        </button>
        <div class="hidden items-center flex-row text-base lg:flex ">
          <button class="focus:outline-none inline-flex px-4 items-center h-full flex-row hover:bg-blue-500">
            <p class="text-white font-bold leading-none tracking-normal">
              Game
            </p>
            <span class="material-icons">
            expand_more
            </span>
          </button>
          <button class="focus:outline-none inline-flex px-6 items-center h-full  hover:bg-blue-500">
            <p class="text-white font-bold leading-none tracking-normal">
              News
            </p>
          </button>
          <button class="focus:outline-none inline-flex px-6 items-center h-full hover:bg-blue-500">
            <p class="text-white font-bold leading-none tracking-normal">
              Forum
            </p>
          </button>
          <div class="focus:outline-none inline-flex px-6 items-center h-full hover:bg-blue-500">
            <p class="text-white font-bold leading-none tracking-normal">
              Support
            </p>
          </div>
          <div class="focus:outline-none inline-flex px-6 items-center h-full flex-row hover:bg-blue-500">
            <p class="text-white font-bold leading-none tracking-normal">
              Shop
            </p>
            <span class="material-icons">
            expand_more
            </span>
          </div>
          <button class="focus:outline-none inline-flex px-4 items-center h-full hover:bg-blue-500">
            <p class="text-blue-300 leading-none tracking-normal">
              Aion Classic
            </p>
          </button>
        </div>
      </div>

      <!--invisible element for positioning-->
      <div class=" invisible items-center text-white lg:hidden sm:flex ">
          <span class="material-icons">
          menu
          </span>
        </div>
      <!--end-->

      <div class="hidden h-full items-center flex-row space-x-6 lg:flex ">
        <button class="flex focus:outline-none">
          <p class="text-white font-bold leading-none tracking-normal">
            LOG IN
          </p>
        </button>
        <button
          class=" focus:outline-none inline-flex items-center justify-center px-12 bg-no-repeat bg-right w-auto h-full bg-play-now1 hover:bg-play-now2"
        >
          <p
            class="font-bold text-xl leading-none tracking-normal text-center text-white"
          >
            PLAY FREE NOW
          </p>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        modal: false,
      };
    },
  };
</script>

<style scoped></style>
