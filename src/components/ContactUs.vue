<script setup lang="ts">
import Button from "./ui/button/Button.vue";
</script>

<template>
  <div class="">
    <div class="mx-auto grid max-w-[1080px] gap-10">
      <div class="grid gap-2">
        <h3
          class="break-words text-center text-[26px] font-bold leading-7 tracking-wide text-[#03B4CB] md:text-start"
        >
          Fordern Sie jetzt Ihr maßgeschneidertes Angebot an
        </h3>
        <p class="text-center font-light leading-7 tracking-wide md:text-start">
          Wir verstehen, dass jedes Gebäude und jede Reinigungsaufgabe ihre
          eigenen Anforderungen hat. Deshalb bieten wir maßgeschneiderte
          Reinigungslösungen, die speziell auf Ihre Bedürfnisse zugeschnitten
          sind. Lassen Sie uns gemeinsam herausfinden, wie wir Ihr Umfeld nicht
          nur sauberer, sondern auch gesünder und angenehmer gestalten können.
        </p>
        <p class="text-center md:text-start">
          <b
            >Kontaktieren Sie uns einfach über das nebenstehende Formular oder
            direkt per:
          </b>
        </p>
      </div>

      <div class="flex items-center justify-center gap-4">
        <Button>WhatsApp</Button>
        <span>oder</span>
        <Button>E-mail schreiben</Button>
      </div>

      <div class="grid gap-4 text-center md:text-start">
        <p>
          Wir freuen uns darauf, von Ihnen zu hören und gemeinsam den ersten
          Schritt zu einer saubereren und gesünderen Umgebung zu machen.
        </p>
        <p class="text-center">
          <b>S&N Gebäudereinigung</b>, Edwin-Scharff-Ring 75, 22309 Hamburg
        </p>
      </div>
    </div>
  </div>
</template>
