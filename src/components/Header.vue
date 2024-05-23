<script setup lang="ts">
import { Menu, Mail, Phone, PhoneCall } from "lucide-vue-next";
import { Button } from "@/components/ui/button";
import {
  Dialog,
  DialogContent,
  DialogDescription,
  DialogHeader,
  DialogTitle,
  DialogTrigger,
} from "@/components/ui/dialog";
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip";

const scrollTo = (id: string, behavior: ScrollBehavior = "auto") => {
  const element = document.getElementById(id);
  if (element) {
    element.scrollIntoView({ behavior });
  }
};
</script>

<template>
  <div class="shadow-md">
    <div
      class="mx-auto grid h-20 max-w-[1080px] px-4 transition-all duration-300 ease-in-out lg:h-24 lg:px-28 xl:px-0"
    >
      <div class="flex items-center justify-between">
        <img src="../assets/img/logo.png" class="w-10 lg:w-14" alt="Logo" />

        <!-- MOBILE MENU -->
        <div class="flex lg:hidden">
          <Dialog>
            <DialogTrigger as-child>
              <Menu class="cursor-pointer" />
            </DialogTrigger>

            <DialogContent class="max-w-xs rounded-lg md:max-w-md">
              <DialogHeader>
                <DialogTitle>Wir helfen Ihnen gerne!</DialogTitle>
                <DialogDescription>
                  Hier finden sie uns schnell und einfach.
                </DialogDescription>
              </DialogHeader>

              <div class="grid gap-2.5">
                <Button type="button">
                  <Mail class="mr-2 w-5" /> reinigungsservice@gmail.com
                </Button>
                <Button type="button">
                  <Phone class="mr-2 w-5" /> 01523-5884265
                </Button>
                <Button>WhatsApp</Button>
              </div>
            </DialogContent>
          </Dialog>
        </div>

        <!-- LAPTOP HEADER -->
        <div class="hidden items-center gap-2 lg:flex">
          <TooltipProvider>
            <Tooltip>
              <TooltipTrigger>
                <Button
                  @click="scrollTo('contact-us', 'smooth')"
                  class="text-md font-semibold"
                  ><Mail
                /></Button>
              </TooltipTrigger>
              <TooltipContent>
                <p>reinigungsservice@gmail.com</p>
              </TooltipContent>
            </Tooltip>
          </TooltipProvider>
          <TooltipProvider>
            <Tooltip>
              <TooltipTrigger>
                <Button
                  @click="scrollTo('contact-us', 'smooth')"
                  class="text-md font-semibold"
                  ><PhoneCall
                /></Button>
              </TooltipTrigger>
              <TooltipContent>
                <p>01523-5884265</p>
              </TooltipContent>
            </Tooltip>
          </TooltipProvider>
          <Button class="px-8">WhatsApp</Button>
        </div>
      </div>
    </div>
  </div>
</template>
