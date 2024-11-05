<template>
  <Head>
    <Title>IRIE PIXEL - Contract Web Developer & Front-end Engineer</Title>
    <Meta
      name="description"
      content="Contract Web Developer - JavaScript, React, Vue, Next, Nuxt - Brighton / London / Remote"
    />
  </Head>
  <div class="flex flex-col items-center justify-center h-screen text-white bg-black/95">
    <NuxtImg
      class="mb-8 rounded-full size-[200px] md:size-[300px]"
      src="/iriepixel.webp"
      width="300"
      height="300"
    />

    <div class="glitch-wrapper">
      <h1
        class="relative z-[1] my-4 text-[32px] md:text-[48px] font-bold glitch"
        data-glitch="IRIE PIXEL"
      >
        IRIE PIXEL
      </h1>
    </div>

    <div class="flex flex-col items-center gap-1 mb-6 text-white/70 max-sm:text-[14px]">
      <p class="">Contract Web Developer & Front-end Engineer</p>
      <p class="">JavaScript, React, Vue, Next, Nuxt</p>
      <p class="">Brighton | London | Remote</p>
    </div>

    <a
      class="underline"
      href="mailto:jev@iriepixel.com"
      >Get in touch</a
    >
  </div>
</template>

<style scoped>
.glitch:before,
.glitch:after {
  display: block;
  content: attr(data-glitch);
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0.5;
}

.glitch:before {
  animation: glitch-color 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) both infinite;
  color: #0ff;
  z-index: -1;
}

.glitch:after {
  animation: glitch-color 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) reverse both infinite;
  color: #ff00ff;
  z-index: -2;
}

@keyframes glitch-color {
  0% {
    transform: translate(0);
  }

  10% {
    transform: translate(-5px, 2px);
  }

  20% {
    transform: translate(0px, 5px);
  }

  30% {
    transform: translate(2px, -2px);
  }

  40% {
    transform: translate(4px, -5px);
  }

  50% {
    transform: translate(0);
  }

  to {
    transform: translate(0);
  }
}
</style>
