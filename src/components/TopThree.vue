<script setup lang="ts">
import { HeartHandshake } from "lucide-vue-next";
import { Separator } from "@/components/ui/separator";
</script>

<template>
  <div
    class="mx-auto grid max-w-[1600px] gap-10 rounded-lg bg-white px-3.5 py-14 shadow-lg md:px-24 md:py-20 lg:flex"
  >
    <div class="grid place-items-center rounded-lg px-3">
      <HeartHandshake class="mb-6 scale-150 fill-blue-400 stroke-white" />
      <div class="grid gap-4 text-center">
        <h3 class="text-xl font-semibold">Persönlicher Kundenservice</h3>
        <p class="font-light tracking-wide">
          Individuelle Betreuung durch feste Ansprechpartner garantiert
          maßgeschneiderte Lösungen für Ihre Bedürfnisse.
        </p>
      </div>
    </div>

    <Separator class="lg:hidden" />

    <div class="grid place-items-center rounded-lg px-3">
      <HeartHandshake class="mb-6 scale-150 fill-blue-400 stroke-white" />
      <div class="grid gap-4 text-center">
        <h3 class="text-xl font-semibold">Persönlicher Kundenservice</h3>
        <p class="font-light tracking-wide">
          Individuelle Betreuung durch feste Ansprechpartner garantiert
          maßgeschneiderte Lösungen für Ihre Bedürfnisse.
        </p>
      </div>
    </div>

    <Separator class="lg:hidden" />

    <div class="grid place-items-center rounded-lg px-3">
      <HeartHandshake class="mb-6 scale-150 fill-blue-400 stroke-white" />
      <div class="grid gap-4 text-center">
        <h3 class="text-xl font-semibold">Persönlicher Kundenservice</h3>
        <p class="font-light tracking-wide">
          Individuelle Betreuung durch feste Ansprechpartner garantiert
          maßgeschneiderte Lösungen für Ihre Bedürfnisse.
        </p>
      </div>
    </div>
  </div>
</template>
