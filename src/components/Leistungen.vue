<script setup lang="ts">
import Card from "../components/Card.vue";
</script>

<template>
  <!-- Container for the entire section with responsive maximum width and spacing -->
  <div class="mx-auto grid max-w-[1080px] gap-4 lg:gap-8">
    <!-- Header section with title and description -->
    <div class="grid gap-3">
      <h3
        class="break-words text-center text-[26px] font-bold leading-7 tracking-wide text-primary"
      >
        Unsere Leistungen für Gewerbereinigung in Hamburg
      </h3>
      <p class="text-center font-light leading-7 tracking-wide">
        S&N Gebäudereinigung steht für maßgeschneiderte Reinigungslösungen mit
        Fokus auf Nachhaltigkeit und Effizienz für Hamburger Gewerbe. Verlassen
        Sie sich auf unsere Expertise für ein hygienisch reines und optisch
        einladendes Geschäftsumfeld.
      </p>
    </div>

    <!-- Grid of services with responsive columns and spacing -->
    <div class="mb-5 grid auto-rows-auto gap-6 md:grid-cols-2 lg:grid-cols-3">
      <!-- Loop to create each service item -->
      <div v-for="i in 9" :key="i" class="relative">
        <div
          class="relative cursor-pointer duration-300 ease-in-out hover:scale-105"
        >
          <img
            src="../assets/img/leistung.jpg"
            class="rounded-lg brightness-50 duration-300 ease-in-out hover:scale-105"
            alt="Leistungen"
          />
          <span
            class="absolute inset-0 flex items-center justify-center text-2xl font-medium tracking-wide text-white"
            >Gebäudereinigung</span
          >
        </div>
      </div>
    </div>

    <!-- Additional services section with highlighted information -->
    <Card
      cardColor="bg-primary"
      cardTitle="Weitere Reinigungsleistungen in Hamburg"
      cardContent="Unser umfassendes Reinigungsangebot deckt eine breite Palette an spezialisierten Dienstleistungen ab, darunter Schul- und Kindergartenreinigung, Fitnessstudio- und Sportanlagenreinigung, Verkehrsmittelreinigung, Restaurantreinigung, Reinigung von Vereinsräumlichkeiten, Eventreinigung und Messereinigung."
    />
  </div>
</template>
