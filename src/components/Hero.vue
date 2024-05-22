<script setup lang="ts">
import { ClipboardList } from "lucide-vue-next";
import { NotebookPen } from "lucide-vue-next";

import Button from "./ui/button/Button.vue";
</script>

<template>
  <div
    class="mx-auto grid max-w-[1080px] items-center px-4 md:px-20 lg:flex lg:items-center lg:px-24 xl:px-0"
  >
    <div class="text-center md:text-start">
      <div class="lg:flex lg:items-center lg:gap-20">
        <div>
          <p class="mb-8 font-semibold md:text-lg">
            Willkommen bei S&N Gebäudereinigung
          </p>
          <h1 class="mb-6 text-[40px] font-extrabold leading-10">
            WEIL SAUBER NICHT GLEICH SAUBER IST
          </h1>
          <p class="font-light leading-7 tracking-wide md:text-lg">
            Entdecken Sie Reinigung, die über das Sichtbarew hinausgeht:
            <b>Qualität, Flexibilität</b> und <b>Nachhaltigkeit</b> in jedem
            Schritt. In Hamburg sind wir Ihr verlässlicher Partner für eine
            saubere Umwelt und Zufriedenheit.
          </p>
        </div>

        <img
          src="../assets/img/cleaning.png"
          class="hidden lg:block lg:h-80 xl:h-96"
          alt=""
        />
      </div>

      <div class="mt-8 grid place-items-center gap-2 md:flex xl:mt-0">
        <Button class="w-fit px-8"
          ><NotebookPen class="mr-2 w-5" />Angebot anfordern
        </Button>
        <Button class="w-fit px-8"
          ><ClipboardList class="mr-2 w-5" />Unsere Leistungen
        </Button>
      </div>

      <img src="../assets/img/cleaning.png" class="lg:hidden" alt="" />
    </div>
  </div>
</template>
