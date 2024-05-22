<script setup lang="ts">
import { HeartHandshake, PhoneCall } from "lucide-vue-next";
import Button from "./ui/button/Button.vue";
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1080px]">
      <h1
        class="mb-10 break-words text-center text-[26px] font-bold leading-7 tracking-wide text-[#03B4CB]"
      >
        Ihre Vorteile bei S&N Gebäuderinigung auf einen Blick
      </h1>

      <div class="mb-5 grid gap-6 lg:grid-cols-3">
        <div
          v-for="i in 3"
          :key="i"
          class="grid place-items-center rounded-lg border-2 border-[#02B4CB] px-5 py-7 md:px-7 md:py-10"
        >
          <HeartHandshake class="mb-6 scale-150 fill-blue-400 stroke-white" />
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

      <div
        class="grid place-items-center rounded-lg bg-[#03B4CB] px-3.5 py-12 md:px-10 md:py-12 lg:flex lg:gap-44"
      >
        <div class="grid place-items-center text-center lg:place-items-start">
          <div class="grid place-items-center lg:flex lg:items-center lg:gap-6">
            <PhoneCall class="mb-6 scale-150 fill-blue-400 stroke-white" />
            <h3 class="mb-4 text-2xl font-bold tracking-wide text-white">
              Jetzt Kontakt aufnehmen
            </h3>
          </div>
          <p
            class="mb-10 text-center font-light leading-7 tracking-wide text-white lg:mb-0 lg:text-start"
          >
            Bereit für eine makellose Geschäftsumgebung? Kontaktieren Sie uns
            jetzt per Telefon oder E-mail, um Ihre individuelle Reinigungslösung
            zu besprechen. Unser Team erwartet Sie, um Ihr Gewerbe zum Strahlen
            zu bringen.
          </p>
        </div>

        <div class="flex gap-2 lg:grid">
          <Button class="bg-white text-[#03B4CB]">01523-5884265</Button>
          <Button class="bg-white text-[#03B4CB]">E-mail</Button>
        </div>
      </div>
    </div>
  </div>
</template>
