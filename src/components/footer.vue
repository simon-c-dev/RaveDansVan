<script setup>
const currentYear = new Date().getFullYear();
</script>

<template>
  <footer class="footer bg-surface-900 text-surface-200">
    <div class="container mx-auto py-4 text-center">
      <p class="text-sm">&copy; {{ currentYear }} Rave Dans Van. Tous droits réservés.</p>
      <div class="flex justify-center space-x-4 mt-2">
        <a href="https://www.facebook.com" target="_blank" class="hover:text-primary-600">
          <font-awesome-icon :icon="['fab', 'facebook']" />
        </a>
        <a href="https://www.twitter.com" target="_blank" class="hover:text-primary-600">
          <font-awesome-icon :icon="['fab', 'twitter']" />
        </a>
        <a href="https://www.instagram.com" target="_blank" class="hover:text-primary-600">
          <font-awesome-icon :icon="['fab', 'instagram']" />
        </a>
      </div>
    </div>
  </footer>
</template>

<style>
.footer {
  position: relative;
  z-index: 10; /* Assure qu'il passe devant */
}
</style>