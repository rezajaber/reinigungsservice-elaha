<script setup lang="ts">
import { SearchCheck, ClipboardList, HeartHandshake } from "lucide-vue-next";

import Button from "./ui/button/Button.vue";

const vorteile = [
  {
    id: 1,
    icon: "SearchCheck",
    title: "Unsere Präzision",
    description:
      "Unsere Arbeit zeichnet sich durch höchste Präzision aus, um sicherzustellen, dass jede Aufgabe mit äußerster Genauigkeit und Sorgfalt ausgeführt wird.",
  },
  {
    id: 2,
    icon: "ClipboardList",
    title: "Unsere Flexibilität",
    description:
      "Dank unserer Vielfalt an Services und unserer Flexibilität können wir uns leicht an die spezifischen Anforderungen unserer Kunden anpassen und maßgeschneiderte Lösungen liefern.",
  },
  {
    id: 3,
    icon: "HeartHandshake",
    title: "Unser Kundenservice",
    description:
      "Wir legen großen Wert auf exzellenten Kundenservice, um sicherzustellen, dass unsere Kunden jederzeit zufrieden sind. Unser engagiertes Team steht Ihnen zur Seite, um Ihre Anliegen zu hören und Ihnen zu helfen.",
  },
];

const icons = [SearchCheck, ClipboardList, HeartHandshake];
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1080px]">
      <div class="grid gap-6 lg:grid-cols-3">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="flex flex-col items-center rounded-lg bg-white px-5 py-7 shadow-lg md:px-7 md:py-10"
        >
          <component
            :is="icons[index]"
            class="mb-4 scale-150 fill-white stroke-primary"
          />
          <h3
            class="mb-2 text-center text-xl font-semibold leading-7 tracking-wide"
          >
            {{ vorteil.title }}
          </h3>
          <p class="text-center font-light leading-7 tracking-wide">
            {{ vorteil.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
