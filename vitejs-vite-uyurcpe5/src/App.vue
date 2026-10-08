<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Programs from './components/Programs.vue'
import FacultyStaff from './components/FacultyStaff.vue'
import Partnerships from './components/Partnerships.vue'
</script>

<template>
  <div>
    <Navbar />

    <main>
      <Hero />
      <Programs />
      <FacultyStaff />
      <Partnerships />
    </main>

    <footer class="footer">
      <p>© 2026 College of Computer Studies</p>
      <p>Central Philippine University</p>
    </footer>
  </div>
</template>