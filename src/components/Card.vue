<script setup lang="ts">
import { EllipsisVertical } from "lucide-vue-next";

const props = defineProps({
  cardTitle: {
    type: String,
    required: true,
  },
  cardContent: {
    type: String,
    required: true,
  },
  cardColor: {
    type: String,
    required: true,
    default: "bg-white",
  },
});
</script>

<template>
  <div
    :class="`grid gap-4 rounded-lg ${props.cardColor} px-3.5 py-10 text-center md:p-10 md:text-start`"
  >
    <div class="flex items-center justify-center gap-1 md:justify-start">
      <EllipsisVertical class="hidden stroke-[#03B4CB] md:block" />
      <p class="text-xl font-semibold">
        {{ props.cardTitle }}
      </p>
    </div>
    <p class="break-words text-lg font-light leading-7">
      {{ props.cardContent }}
    </p>
  </div>
</template>
