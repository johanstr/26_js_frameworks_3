<script setup>
import { onBeforeMount } from 'vue'
import { useGamesStore } from '@/stores/games'
import { RouterView } from 'vue-router'
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'

const store = useGamesStore();

onBeforeMount( () => {
   store.loadGames();
   console.log(store.getGames);
} );
</script>

<template>
   <Nav />

   <main>
      <div class="album py-5 bg-body-tertiary">
      <RouterView />
      </div>
   </main>

   <Footer />
</template>

<style scoped>

</style>
