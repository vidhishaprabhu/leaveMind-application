<template>
  <div class="app-layout">
    <AppSidebar />
    <div class="content">
      <router-view />
    </div>
  </div>
</template>

<script>
import AppSidebar from './components/AppSidebar.vue'
export default {
  name: 'App',
  components:{ AppSidebar }
}
</script>

<style>

</style>
