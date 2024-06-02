<script setup lang="ts"></script>

<template>
  <div
    class="mx-auto grid max-w-[1080px] place-items-center gap-6 rounded-lg border-2 border-[#02B4CB] bg-white px-3 py-14 md:px-10 lg:flex lg:gap-14 xl:gap-24"
  >
    <!-- LOGO (Mobile) -->
    <img
      src="../assets/img/logo.png"
      alt="Logo"
      class="w-52 md:w-80 lg:hidden"
    />

    <!-- STAR RATING AND TEXT -->
    <div class="grid place-items-center gap-6 md:place-items-start">
      <!-- STAR RATING -->
      <div class="grid gap-1 text-center text-sm font-light md:text-start">
        <p>Top Service für Sie</p>
        <div class="flex items-center">
          <svg
            class="me-1 h-4 w-4 text-[#F0AD4E]"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 22 20"
          >
            <path
              d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
            />
          </svg>
          <svg
            class="me-1 h-4 w-4 text-[#F0AD4E]"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 22 20"
          >
            <path
              d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
            />
          </svg>
          <svg
            class="me-1 h-4 w-4 text-[#F0AD4E]"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 22 20"
          >
            <path
              d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
            />
          </svg>
          <svg
            class="me-1 h-4 w-4 text-[#F0AD4E]"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 22 20"
          >
            <path
              d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
            />
          </svg>
          <svg
            class="me-1 h-4 w-4 text-gray-400 dark:text-gray-500"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 22 20"
          >
            <path
              d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z"
            />
          </svg>
          <p class="ms-1 text-sm font-medium text-gray-500 dark:text-gray-400">
            4.95
          </p>
          <p class="ms-1 text-sm font-medium text-gray-500 dark:text-gray-400">
            out of
          </p>
          <p class="ms-1 text-sm font-medium text-gray-500 dark:text-gray-400">
            5
          </p>
        </div>
      </div>

      <!-- TEXT -->
      <h1
        class="break-words text-center text-[26px] font-bold leading-7 tracking-wide text-primary md:text-start"
      >
        Willkommen bei S&N Gebäudereinigung Hamburg
      </h1>

      <p class="text-center font-light leading-7 tracking-wide md:text-start">
        S&N Gebäudereinigung in Hamburg steht für Professionalität, Qualität und
        Nachhaltigkeit in der Gebäudereinigungsbranche. Mit jahrelanger
        Erfahrung und einem Team aus geschulten Fachkräften bieten wir ein
        breites Spektrum an Reinigungsdienstleistungen an, von der Büro- bis zur
        Industriereinigung, alles unter Berücksichtigung ökologischer Standards.
        Unsere Mission ist es, durch erstklassigen Service und umweltfreundliche
        Reinigungsmethoden zur Wohlfühlatmosphäre und Werterhaltung Ihrer
        Immobilien beizutragen.
      </p>
    </div>

    <!-- LOGO (Desktop) -->
    <img
      src="../assets/img/logo-grid.svg"
      alt="Logo"
      class="hidden w-52 lg:block"
    />
  </div>
</template>
