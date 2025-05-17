<template>
  <div id="app" class="min-h-screen flex flex-col">
    <!-- Header -->
    <ComHeader />

    <!-- Main Content with Transition -->
    <main class="flex-grow">
      <transition name="fade" mode="out-in">
        <router-view />
      </transition>
    </main>

    <!-- Footer -->
    <ComFooter />
  </div>
</template>

<script>
import ComHeader from './components/ComHeader.vue'
import ComFooter from './components/ComFooter.vue'

export default {
  name: 'App',
  components: {
    ComHeader,
    ComFooter
  }
}
</script>

<style>
/* Base styles */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

/* Page transition animation */
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s ease;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>
