<script setup lang="ts">
import { HeartHandshake } from "lucide-vue-next";
import Button from "./ui/button/Button.vue";
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1080px]">
      <h1
        class="mb-10 break-words text-center text-[26px] font-bold leading-7 tracking-wide text-primary"
      >
        Ihre Vorteile bei S&N Gebäuderinigung auf einen Blick
      </h1>

      <div class="mb-5 grid gap-6 lg:grid-cols-3">
        <div
          v-for="i in 3"
          :key="i"
          class="grid place-items-center rounded-lg border-2 border-primary px-5 py-7 md:px-7 md:py-10"
        >
          <HeartHandshake class="mb-6 scale-150 fill-white stroke-primary" />
          <h3
            class="mb-2 text-center text-xl font-semibold leading-7 tracking-wide"
          >
            Eigenes Reinigungsequipment
          </h3>
          <p class="text-center font-light leading-7 tracking-wide">
            Wir setzen auf unsere eigenen, hochwertigen Reinigungsprodukte und
            -geräte für erstklassige Sauberkeit.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
