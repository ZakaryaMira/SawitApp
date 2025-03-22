<template>
  <div>
    <NavHome />
    <Home />
  </div>
</template>

<script>
import NavHome from '@/components/HomePageComponents/NavHome.vue'
import Home from '@/components/HomePageComponents/Home.vue'

export default {
  components: {
    NavHome,
    Home,
  },
}
</script>
