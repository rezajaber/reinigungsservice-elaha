<script setup lang="ts">
import { ClipboardList, NotebookPen } from "lucide-vue-next";
import Button from "./ui/button/Button.vue";
</script>

<template>
  <div class="relative isolate">
    <!-- Gradient background -->
    <div
      class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80"
      aria-hidden="true"
    >
      <div
        class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-[#0ff] to-[#0f0] opacity-30 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]"
        style="
          clip-path: polygon(
            74.1% 44.1%,
            100% 61.6%,
            97.5% 26.9%,
            85.5% 0.1%,
            80.7% 2%,
            72.5% 32.5%,
            60.2% 62.4%,
            52.4% 68.1%,
            47.5% 58.3%,
            45.2% 34.5%,
            27.5% 76.7%,
            0.1% 64.9%,
            17.9% 100%,
            27.6% 76.8%,
            76.1% 97.7%,
            74.1% 44.1%
          );
        "
      ></div>
    </div>

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
              Entdecken Sie Reinigung, die über das Sichtbare hinausgeht:
              <b>Qualität, Flexibilität</b> und <b>Nachhaltigkeit</b> in jedem
              Schritt. In Hamburg sind wir Ihr verlässlicher Partner für eine
              saubere Umwelt und Zufriedenheit.
            </p>
          </div>
          <img
            src="../assets/img/cleaning.png"
            class="hidden lg:block lg:h-80 xl:h-96"
            alt="Cleaning"
          />
        </div>

        <div
          class="mt-8 grid place-items-center gap-2 md:flex lg:-mt-2 xl:-mt-12"
        >
          <Button class="w-fit px-8">
            <NotebookPen class="mr-2 w-5" />Angebot anfordern
          </Button>
          <Button class="w-fit px-8">
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
