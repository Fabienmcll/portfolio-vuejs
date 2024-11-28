<template>
  <div>
    <Navbar />
    <Profile />
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';
import Profile from '@/components/Profile.vue';
import Footer from "@/components/Footer.vue";
export default {
  name: 'Home',
  components: {
    Navbar,
    Profile,
    Footer
  },
};
</script>

<style scoped>
</style>
