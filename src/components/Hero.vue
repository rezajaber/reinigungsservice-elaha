<script setup lang="ts">
import { ClipboardList, NotebookPen } from "lucide-vue-next";
import Button from "./ui/button/Button.vue";

const scrollTo = (id: string, behavior: ScrollBehavior = "auto") => {
  const element = document.getElementById(id);
  if (element) {
    element.scrollIntoView({ behavior });
  }
};
</script>

<template>
  <div class="relative isolate">
    <div
      class="mx-auto grid max-w-[1080px] items-center px-4 md:px-20 lg:flex lg:items-center lg:px-24 xl:px-0"
    >
      <div class="text-center md:text-start">
        <div class="lg:flex lg:items-center lg:gap-20">
          <div>
            <p class="mb-8 font-semibold md:text-lg">
              Herzlichen Willkommen bei N&T-Reinungsfirma
            </p>
            <h1 class="mb-6 text-[40px] font-extrabold leading-10">
              WEIL SAUBERKEIT VERTRAUEN SCHAFFT
            </h1>
            <p class="font-light leading-7 tracking-wide md:text-lg">
              Tauchen Sie ein in eine Welt der Sauberkeit, die überzeugt:
              <b>Präzision, Flexibilität</b> und <b>Nachhaltigkeit</b> bei jedem
              Auftrag. Wir bieten verlässliche Sauberkeit, Kundenzufriedenheit.
            </p>
          </div>
          <img
            src="../assets/img/cleaning.png"
            class="hidden lg:block lg:h-80 xl:h-96"
            alt="Cleaning"
          />
        </div>

        <div
          class="mt-8 grid place-items-center gap-2 md:flex lg:mt-2 xl:-mt-12"
        >
          <Button @click="scrollTo('contact-us', 'smooth')">
            <NotebookPen class="mr-2 w-5" />Angebot anfordern
          </Button>
          <Button @click="scrollTo('leistungen', 'smooth')">
            <ClipboardList class="mr-2 w-5" />Unsere Leistungen
          </Button>
        </div>

        <img
          src="../assets/img/cleaning.png"
          class="lg:hidden"
          alt="Cleaning"
        />
      </div>
    </div>
  </div>
</template>
