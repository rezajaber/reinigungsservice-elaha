<script setup lang="ts">
import { Menu, Mail, Phone } from "lucide-vue-next";

import { Button } from "@/components/ui/button";
import {
  Dialog,
  DialogClose,
  DialogContent,
  DialogDescription,
  DialogFooter,
  DialogHeader,
  DialogTitle,
  DialogTrigger,
} from "@/components/ui/dialog";
</script>

<template>
  <div class="grid h-20 px-4">
    <div class="flex items-center justify-between">
      <img src="../assets/img/logo.svg" class="w-48" alt="Logo" />

      <div class="flex">
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
                <Mail class="mr-2 w-5" />reinigungsservice@gmail.com
              </Button>

              <Button type="button" variant="secondary">
                <Phone class="mr-2 w-5" />01523-5884265
              </Button>

              <Button class="bg-green-700">WhatsApp</Button>
            </div>
          </DialogContent>
        </Dialog>
      </div>
    </div>
  </div>
</template>
