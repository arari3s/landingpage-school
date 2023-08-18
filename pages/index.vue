<template>
  <div>
    <div class="hero-bg">
      <div
        class="mx-auto flex pt-16 pb-16 lg:pb-20 lg:px-24 md:px-16 sm:px-8 px-8 lg:flex-row flex-col"
      >
        <!-- Left Column -->
        <div
          class="lg:flex-grow lg:w-1/2 flex flex-col lg:items-start lg:text-left mb-3 md:mb-12 lg:mb-0 items-center text-center"
        >
          <h1
            class="text-slate-800 lg:leading-normal sm:text-4xl lg:text-5xl text-3xl mb-5 lg:mt-20"
          >
            Mulai Kebiasaan Baru, <br class="lg:block hidden" />
            Tanpa <span class="font-bold">Banyak Alasan</span>
          </h1>
          <p
            class="text-lg leading-relaxed text-slate-500 font-light tracking-wide mb-10 lg:mb-18"
          >
            #bpSmart
          </p>
        </div>

        <!-- Right Column -->
        <div
          class="w-full lg:w-1/2 text-center lg:justify-start justify-center flex pr-0"
        >
          <img
            class="bottom-0 lg:block lg:right-24 md:right-16 sm:right-8 right-8 w-75"
            src="/assets/hero-image.png"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'dashboard',
}
</script>
