<script setup lang="ts">
import Card from "../components/Card.vue";
</script>

<template>
  <!-- Container for the entire section with responsive maximum width and spacing -->
  <div class="mx-auto grid max-w-[1080px] gap-4 lg:gap-6">
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
    <div class="grid auto-rows-auto gap-6 md:grid-cols-2 lg:grid-cols-3">
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
      cardTitle="Individuelle Reinigungslösungen für jeden Bedarf"
      cardContent="Obwohl unser umfassendes Reinigungsangebot eine Vielzahl spezialisierter Dienstleistungen umfasst – von Schul- und Kindergartenreinigung über Fitnessstudio- und Sportanlagenreinigung bis hin zur Verkehrsmittelreinigung, Restaurantreinigung, Reinigung von Vereinsräumlichkeiten, Eventreinigung und Messereinigung – verstehen wir, dass Ihre Anforderungen möglicherweise darüber hinausgehen könnten. Wenn Sie also spezifische Reinigungsdienstleistungen benötigen, die hier nicht aufgeführt sind, zögern Sie nicht, uns zu kontaktieren. Unser erfahrenes Team steht Ihnen gerne zur Verfügung, um individuelle Reinigungslösungen zu entwickeln, die genau auf Ihre Bedürfnisse zugeschnitten sind."
    />
  </div>
</template>
