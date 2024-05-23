<script setup lang="ts">
import { ListChecks } from "lucide-vue-next";
import Card from "../components/Card.vue";
</script>

<template>
  <div>
    <!-- ENGAGEMENT TEXT -->
    <div
      class="mx-auto mb-8 grid max-w-[1080px] gap-6 text-center md:text-start"
    >
      <h3
        class="break-words text-[26px] font-bold leading-7 tracking-wide text-[#03B4CB]"
      >
        Unser Engagement für Ihre Zufriedenheit
      </h3>
      <p class="font-light leading-7 tracking-wide">
        In einer Welt, in der <b>Sauberkeit</b> und Wohlbefinden Hand in Hand
        gehen, steht unser Unternehmen für
        <b>maßgeschneiderte Reinigungslösungen</b>, die genau auf Ihre
        Bedürfnisse zugeschnitten sind. Als ein kleineres Unternehmen legen wir
        großen Wert auf persönlichen Kontakt und <b>direkte Kommunikation</b>,
        um unseren Service kontinuierlich an Ihre Wünsche anzupassen. Entdecken
        Sie unser Engagement für Qualität, Fairness und Umweltschutz.
      </p>
    </div>

    <!-- CARDS -->
    <div class="mx-auto grid max-w-[1080px] gap-6">
      <div class="flex items-center gap-10">
        <Card
          cardTitle="Weitere Reinigungsleistungen in Hamburg"
          cardContent="Unser umfassendes Reinigungsangebot deckt eine breite Palette an spezialisierten Dienstleistungen ab, darunter Schul- und Kindergartenreinigung, Fitnessstudio- und Sportanlagenreinigung, Verkehrsmittelreinigung, Restaurantreinigung, Reinigung von Vereinsräumlichkeiten, Eventreinigung und Messereinigung."
        />

        <ListChecks class="hidden h-auto w-80 stroke-[#C8EBF0] lg:block" />
      </div>

      <div class="flex items-center gap-10">
        <ListChecks class="hidden h-auto w-80 stroke-[#C8EBF0] lg:block" />

        <Card
          cardTitle="Weitere Reinigungsleistungen in Hamburg"
          cardContent="Unser umfassendes Reinigungsangebot deckt eine breite Palette an spezialisierten Dienstleistungen ab, darunter Schul- und Kindergartenreinigung, Fitnessstudio- und Sportanlagenreinigung, Verkehrsmittelreinigung, Restaurantreinigung, Reinigung von Vereinsräumlichkeiten, Eventreinigung und Messereinigung."
        />
      </div>

      <div class="flex items-center gap-10">
        <Card
          cardTitle="Weitere Reinigungsleistungen in Hamburg"
          cardContent="Unser umfassendes Reinigungsangebot deckt eine breite Palette an spezialisierten Dienstleistungen ab, darunter Schul- und Kindergartenreinigung, Fitnessstudio- und Sportanlagenreinigung, Verkehrsmittelreinigung, Restaurantreinigung, Reinigung von Vereinsräumlichkeiten, Eventreinigung und Messereinigung."
        />

        <ListChecks class="hidden h-auto w-80 stroke-[#C8EBF0] lg:block" />
      </div>
    </div>
  </div>
</template>
