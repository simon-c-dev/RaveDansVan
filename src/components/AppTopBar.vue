<template>
  <Disclosure as="nav" class="bg-transparent w-full fixed top-0 left-0 z-50" v-slot="{ open }">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-16 items-center justify-between">
        <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400
          hover:bg-gray-700 hover:text-white
          focus:ring-2 focus:ring-white focus:outline-hidden focus:ring-inset">
            <span class="absolute -inset-0.5" />
            <span class="sr-only">Open main menu</span>
            <Bars3Icon v-if="!open" class="block size-6" aria-hidden="true" />
            <XMarkIcon v-else class="block size-6" aria-hidden="true" />
          </DisclosureButton>
        </div>
        <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
          <div class="flex shrink-0 items-center">
            <span class="text-2xl sm:text-4xl text-primary ml-2" id="rdv">RDV</span>
          </div>
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4">
              <a v-for="item in navigation" :key="item.name" :href="item.href"
                 class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md
                  px-3 py-2 text-sm font-medium">{{ item.name }}
              </a>
            </div>
          </div>
        </div>
        <div class="absolute gap-1 inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">
          <a v-for="item in social" :href="item.href" target="_blank" class="relative p-1 text-primary-600 hover:text-white">
            <span class="absolute -inset-1.5" />
            <span class="sr-only">{{ item.name }} link</span>
            <font-awesome-icon :icon="item.icon" />
          </a>
        </div>
      </div>
    </div>

    <DisclosurePanel class="sm:hidden">
      <div class="space-y-1 px-2 pt-2 pb-3">
        <DisclosureButton v-for="item in navigation" :key="item.name" as="a" :href="item.href"
                          class="text-gray-300 hover:bg-gray-700 hover:text-white block
                          rounded-md px-3 py-2 text-base font-medium']">{{ item.name }}
        </DisclosureButton>
      </div>
    </DisclosurePanel>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
import { Bars3Icon, XMarkIcon } from '@heroicons/vue/24/outline'

const navigation = [
  { name: 'Événements', href: '#' },
  { name: 'Merch', href: '#' },
  { name: 'Radio', href: '#' },
  { name: 'Médias', href: '#' },
]

const social = [
  {name: 'Instagram', href: 'https://www.instagram.com', icon: "fa-brands fa-instagram"},
  {name: 'Shopify', href: 'https://www.shopify.com', icon: "fa-brands fa-shopify"},
  {name: 'Patreon', href: 'https://www.patreon.com', icon: "fa-brands fa-patreon"},
]

</script>

<style scoped>
#rdv{
  font-family: saira,serif;
}
</style>