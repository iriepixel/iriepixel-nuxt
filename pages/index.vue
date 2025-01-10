<script setup lang="ts"></script>

<template>
  <div class="flex flex-col items-center justify-center min-h-screen text-white bg-black/95 py-20">
    <NuxtImg
      class="mb-4 md:mb-8 rounded-full size-[200px] md:size-[300px]"
      src="/iriepixel.webp"
      width="300"
      height="300"
    />

    <div class="glitch-wrapper">
      <h1
        class="relative z-[1] my-4 text-[32px] md:text-[48px] font-bold glitch"
        data-glitch="Jev"
      >
        Jev
      </h1>
    </div>

    <div class="flex flex-col items-center gap-1 mb-6 text-white/70 max-md:text-[14px]">
      <p class="">Contract Web Developer & Front-end Engineer</p>
      <p class="">JavaScript, React, Vue, Next, Nuxt</p>
      <p class="">Brighton | London | Remote</p>
    </div>

    <a
      class="underline"
      href="mailto:jev@iriepixel.com"
      >Get in touch</a
    >

    <div class="mt-10">
      <h2 class="text-center mb-4 text-white/20 text-[14px]">Recent Work</h2>
      <div
        class="flex flex-col md:flex-row max-md:divide-y md:divide-x divide-solid divide-white/10 max-md:text-[14px] text-center text-white/70"
      >
        <NuxtLink
          class="max-md:py-2 md:px-4 hover:underline"
          to="https://timothy.london"
          target="_blank"
        >
          Timothy London
        </NuxtLink>
        <NuxtLink
          class="max-md:py-2 md:px-4 hover:underline"
          to="https://www.alfasystems.com"
          target="_blank"
        >
          Alfa Systems
        </NuxtLink>
        <NuxtLink
          class="max-md:py-2 md:px-4 hover:underline"
          to="https://www.fairr.org"
          target="_blank"
        >
          Fairr
        </NuxtLink>
        <NuxtLink
          class="max-md:py-2 md:px-4 hover:underline"
          to="https://www.ussif.org"
          target="_blank"
        >
          US SIF
        </NuxtLink>
        <NuxtLink
          class="max-md:py-2 md:px-4 hover:underline"
          to="https://investors.pod-point.com/"
          target="_blank"
        >
          Pod Point
        </NuxtLink>
      </div>
    </div>
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
