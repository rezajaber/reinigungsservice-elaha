<script setup lang="ts">
import { HeartHandshake, PhoneCall } from "lucide-vue-next";
import Button from "./ui/button/Button.vue";
</script>

<template>
  <div class="">
    <div class="mx-auto grid max-w-[1080px] gap-10">
      <div class="grid gap-5 text-white">
        <h3
          class="break-words text-center text-[26px] font-bold leading-7 tracking-wide md:text-start"
        >
          Fordern Sie jetzt Ihr maßgeschneidertes Angebot an
        </h3>
        <p
          class="text-center font-light leading-7 tracking-wide opacity-90 md:text-start"
        >
          Wir verstehen, dass jedes Gebäude und jede Reinigungsaufgabe ihre
          eigenen Anforderungen hat. Deshalb bieten wir maßgeschneiderte
          Reinigungslösungen, die speziell auf Ihre Bedürfnisse zugeschnitten
          sind. Lassen Sie uns gemeinsam herausfinden, wie wir Ihr Umfeld nicht
          nur sauberer, sondern auch gesünder und angenehmer gestalten können.
        </p>
        <p class="text-center opacity-90 md:text-start">
          <b
            >Kontaktieren Sie uns einfach über das nebenstehende Formular oder
            direkt per:
          </b>
        </p>
      </div>

      <div
        class="grid place-items-center rounded-lg bg-secondary px-3.5 py-12 md:px-10 md:py-12 lg:flex lg:gap-44"
      >
        <div
          class="grid place-items-center gap-4 text-center lg:place-items-start"
        >
          <div class="grid place-items-center lg:flex lg:items-center lg:gap-4">
            <PhoneCall class="fill-primary stroke-primary" />
            <h3 class="text-2xl font-bold tracking-wide text-primary">
              Jetzt Kontakt aufnehmen
            </h3>
          </div>
          <p
            class="mb-10 text-center font-light leading-7 tracking-wide text-primary lg:mb-0 lg:text-start"
          >
            Bereit für eine makellose Geschäftsumgebung? Kontaktieren Sie uns
            jetzt per Telefon oder E-mail, um Ihre individuelle Reinigungslösung
            zu besprechen. Unser Team erwartet Sie, um Ihr Gewerbe zum Strahlen
            zu bringen.
          </p>
        </div>

        <div class="flex gap-2 lg:grid">
          <Button class="bg-primary text-white">01523-5884265</Button>
          <Button class="bg-primary text-white">E-mail</Button>
        </div>
      </div>
    </div>
  </div>
</template>
