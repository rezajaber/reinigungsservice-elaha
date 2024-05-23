<script setup lang="ts">
import { SearchCheck, ClipboardList, HeartHandshake } from "lucide-vue-next";
import { Separator } from "@/components/ui/separator";

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
  <div
    class="mx-auto max-w-[1600px] rounded-lg bg-white px-3.5 py-14 shadow-lg md:px-24 md:py-20 lg:flex lg:justify-between"
  >
    <div
      v-for="(vorteil, index) in vorteile"
      :key="vorteil.id"
      class="flex flex-col items-center rounded-lg px-5 py-7 md:px-7 md:py-10 lg:w-1/3"
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
</template>
