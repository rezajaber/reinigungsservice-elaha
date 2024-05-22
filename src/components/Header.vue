<script setup lang="ts">
import { Menu, Mail, Phone } from "lucide-vue-next";
import { Button } from "@/components/ui/button";
import {
  Dialog,
  DialogContent,
  DialogDescription,
  DialogHeader,
  DialogTitle,
  DialogTrigger,
} from "@/components/ui/dialog";
</script>

<template>
  <div class="shadow-md">
    <div
      class="mx-auto grid h-20 max-w-[1080px] px-4 transition-all duration-300 ease-in-out lg:h-28 lg:px-28 xl:px-0"
    >
      <div class="flex items-center justify-between">
        <img src="../assets/img/logo.svg" class="w-48 lg:w-72" alt="Logo" />

        <!-- MOBILE MENU -->
        <div class="flex lg:hidden">
          <Dialog>
            <DialogTrigger as-child>
              <Button variant="ghost"><Menu /></Button>
            </DialogTrigger>

            <DialogContent class="max-w-xs rounded-lg md:max-w-md">
              <DialogHeader>
                <DialogTitle>Wir helfen Ihnen gerne!</DialogTitle>
                <DialogDescription>
                  Hier finden sie uns schnell und einfach.
                </DialogDescription>
              </DialogHeader>

              <div class="grid gap-2.5">
                <Button type="button" variant="secondary">
                  <Mail class="mr-2 w-5" /> reinigungsservice@gmail.com
                </Button>
                <Button type="button" variant="secondary">
                  <Phone class="mr-2 w-5" /> 01523-5884265
                </Button>
                <Button class="bg-green-700">WhatsApp</Button>
              </div>
            </DialogContent>
          </Dialog>
        </div>

        <!-- LAPTOP HEADER -->
        <div class="hidden items-center gap-6 lg:flex">
          <span class="text-md font-semibold">info@sn-hamburg.de</span>
          <span class="text-md font-semibold">0151-283402930</span>
          <Button class="px-8">WhatsApp</Button>
        </div>
      </div>
    </div>
  </div>
</template>
