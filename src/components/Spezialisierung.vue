<script setup lang="ts">
import { Syringe, BriefcaseMedical, GraduationCap } from "lucide-vue-next";

import Button from "./ui/button/Button.vue";

const vorteile = [
  {
    id: 1,
    icon: "Syringe",
    title: "Praxen",
    description:
      "Unsere Arbeit zeichnet sich durch höchste Präzision aus, um sicherzustellen, dass jede Aufgabe mit äußerster Genauigkeit und Sorgfalt ausgeführt wird.",
  },
  {
    id: 2,
    icon: "BriefcaseMedical",
    title: "Apotheken",
    description:
      "Unsere flexiblen Reinigungsservices für Apotheken passen sich Ihren individuellen Bedürfnissen an und sorgen für ein hygienisch einwandfreies und einladendes Geschäftsumfeld. Verlassen Sie sich auf unsere maßgeschneiderten Lösungen für Ihre Apotheke.",
  },
  {
    id: 3,
    icon: "GraduationCap",
    title: " Kitas und Schulen",
    description:
      "Wir sorgen für saubere und sichere Lern- und Spielumgebungen in Kitas und Schulen. Unser engagiertes Team bietet umfassende Reinigungslösungen, die auf die besonderen Bedürfnisse von Bildungseinrichtungen abgestimmt sind.",
  },
];

const icons = [Syringe, BriefcaseMedical, GraduationCap];
</script>

<template>
  <div>
    <div class="mx-auto max-w-[1080px]">
      <div class="mb-5 grid gap-3">
        <h3
          class="break-words text-center text-[26px] font-bold leading-7 tracking-wide text-primary md:text-start"
        >
          Unsere Einsatzbereiche für Gewerbereinigungen in Hamburg
        </h3>
        <p class="text-center font-light leading-7 tracking-wide md:text-start">
          Unsere Reinigungsdienste garantieren höchste Hygienestandards, passen
          sich Ihren individuellen Bedürfnissen an und sorgen für saubere und
          sichere Lern- und Geschäftsumgebungen. Vertrauen Sie auf unsere
          maßgeschneiderten Lösungen für Praxen, Apotheken sowie Kitas und
          Schulen, um ein hygienisch einwandfreies und einladendes Umfeld zu
          schaffen.
        </p>
      </div>

      <div class="grid gap-6 lg:grid-cols-3">
        <div
          v-for="(vorteil, index) in vorteile"
          :key="vorteil.id"
          class="flex flex-col items-center rounded-lg bg-primary px-5 py-7 shadow-lg md:px-7 md:py-10"
        >
          <component :is="icons[index]" class="mb-4 scale-150 stroke-white" />
          <h3
            class="mb-2 text-center text-xl font-semibold leading-7 tracking-wide text-white"
          >
            {{ vorteil.title }}
          </h3>
          <p class="text-center font-light leading-7 tracking-wide text-white">
            {{ vorteil.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
