<template class="">
  <div
    class="flex bg-no-repeat w-full lg:h-screen lg:bg-cover lg:bg-pvp-hero bg-100 sm:bg-pvp-hero-mobile sm:h-84 sm:mt-12"
  >
    <div
      class="static font-medium space-y-4 tracking-normal leading-normal ml-12 font-serif justify-end w-full max-w-55 flex flex-col lg:mb-28 sm:ml-5"
    >
      <h1 class="lining-nums text-7xl sm:text-4.5xl">
        Aion Classic Character Reservation Is Live!
      </h1>
      <p class="text-base">
        One week only! Reserve your character and get a free pet!
      </p>
      <div class="flex pt-4">
        <button
          class="focus:outline-none border-white border  rounded-md py-4 px-6 text-center text-xs w-40 hover:bg-blue-600"
        >
          LOGIN TODAY
        </button>
      </div>
    </div>
  </div>

  <div class=" px-12 w-full sm:px-5 sm:mt-28 pb-12">
    <p class="text-base pb-4">LATEST NEWS & UPDATES</p>
    <div class="grid text-center lg:grid-cols-4 h-full gap-4 md:grid-cols-2">
      <div
        class="group text-start rounded-lg overflow-hidden w-full hover:bg-hoverCard transform duration-300 ease-in-out hover:-translate-y-3 md:h-226 "
      >
        <img
          src="../../assets/imgs/news/news1.jpg"
          alt=""
          class="bg-cover object-cover overflow-hidden w-full bg-center border-b-5 border-transparent border-solid duration-200 group-hover:border-card1bb md:h-3/6 "
        />
        <div class="p-4 text-left">
          <p class="tracking-normal">6/16/2021 <span>| General</span></p>
          <p class="text-2xl leading-normal tracking-wide">
            Earn EXCLUSIVE prizes by showing off your creativity!
          </p>
        </div>
      </div>

      <div
        class="group text-start rounded-lg overflow-hidden w-full hover:bg-hoverCard transform duration-300 ease-in-out hover:-translate-y-3 md:h-226 "
      >
        <img
          src="../../assets/imgs/news/news2.jpg"
          alt=""
          class="bg-cover object-cover overflow-hidden w-full bg-center border-b-5 border-transparent border-solid duration-200 group-hover:border-card2bb md:h-3/6 "
        />
        <div class="p-4 text-left">
          <p class="tracking-normal">6/16/2021 <span>| Event</span></p>
          <p class="text-2xl leading-normal tracking-wide">
            Kick Back, Relax and Earn!
          </p>
        </div>
      </div>

      <div
        class="group text-start rounded-lg overflow-hidden w-full hover:bg-hoverCard transform duration-300 ease-in-out hover:-translate-y-3 md:h-226 "
      >
        <img
          src="../../assets/imgs/news/news3.jpg"
          alt=""
          class="bg-cover object-cover overflow-hidden w-full bg-center border-b-5 border-transparent border-solid duration-200 group-hover:border-purple-500 md:h-3/6 "
        />
        <div class="p-4 text-left">
          <p class="tracking-normal">6/15/2021 <span>| Event</span></p>
          <p class="text-2xl leading-normal tracking-wide">
            Everyone likes Ice Cream. But this Ice Cream is Special!
          </p>
        </div>
      </div>

      <div
        class="group text-start rounded-lg overflow-hidden w-full hover:bg-hoverCard transform duration-300 ease-in-out hover:-translate-y-3 md:h-226 "
      >
        <img
          src="../../assets/imgs/news/news4.jpg"
          alt=""
          class="bg-cover object-cover overflow-hidden w-full bg-center border-b-5 border-transparent border-solid duration-200 group-hover:border-pink-500 md:h-3/6 "
        />
        <div class="p-4 text-left">
          <p class="tracking-normal">6/10/2021 <span>| General</span></p>
          <p class="text-2xl leading-normal tracking-wide">
            Get Ready to relive to glory of the past in Aion Classic
          </p>
        </div>
      </div>
    </div>
  </div>

  <div class="flex w-full justify-center pb-12 ">
    <button class="flex flex-row space-x-2 items-center">
      <span class="material-icons font-medium">
        apps
      </span>
      <p class="text-lg">VIEW ALL NEWS</p>
    </button>
  </div>

  <div class="lg:min-h-980 bg-no-repeat w-full h-full lg:bg-center bg-contain bg-balaurea1 lg:bg-cover lg:bg-balaurea1">
    <div class="flex justify-center">
     <img src="../../assets/imgs/balaureaWallpaper.png" alt="" class="w-3/6">
    </div>
    <div class="flex flex-row justify-between px-12">
     <div class="flex flex-col space-y-2">
       <p class="text-5xl font-semibold">Aion: Shadows of Balaurea</p>
       <p class="text-3xl font-medium">Official Trailer</p>
       <p class="text-lg">Get ready to experience brand new Balaurea!</p>
     </div>
     <div class="inline-flex justify-center items-center mr-32">
       <button @click="balaureaTrailer" alt="video play" class="z-10 absolute transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 ">
        <span class="material-icons text-6xl">
        play_circle_outline
        </span>
       </button>
       <img src="../../assets/imgs/balaureaWallpaper2.png" alt="" class="w-226 border-4 border-card1bb">
     </div>
    </div>
  </div>

  <div v-if="openTrailer"
      class="fixed z-50 inset-0 bg-black bg-opacity-50"
    >
      <div @click.self="balaureaTrailer"
        class="flex justify-center min-h-screen items-center p-4 text-center"
      >
        <div
          class=" w-full"
        >
          <div class="flex flex-col h-full ">
            <button @click="balaureaTrailer" class="focus:outline-none flex justify-end w-full items-center">
            <span class="material-icons text-white text-4xl absolute z-20">
              close
            </span>
            </button>
            <div class="aspect-w-13 aspect-h-6.5">
              <iframe src="https://www.youtube.com/embed/O5bdAbCtJps?autoplay=1&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;enablejsapi=1&amp;origin=https%3A%2F%2Fwww.aiononline.com" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>

</template>

<script>
  export default {
    data(){
      return{
        openTrailer: false,
      }
    },

    methods:{
      balaureaTrailer(){
        this.openTrailer = !this.openTrailer
      }
    },
  };
</script>
