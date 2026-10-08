<script setup>
const partnerships = [
  {
    name: 'Technology Industry Partners',
    description:
      'Collaborating with technology organizations to provide students with opportunities for learning and professional development.'
  },

  {
    name: 'Academic Partnerships',
    description:
      'Building relationships with educational institutions to support knowledge sharing, research, and academic activities.'
  },

  {
    name: 'Professional Organizations',
    description:
      'Participating in professional organizations that promote computing education and professional development.'
  },

  {
    name: 'Community Partnerships',
    description:
      'Working with communities through technology-related projects, outreach, and service.'
  }
]
</script>

<template>
  <section id="partnerships" class="section">

    <div class="container">

      <div class="section-heading">
        <p class="eyebrow">COLLABORATION</p>

        <h2>Partnerships & Memberships</h2>

        <p>
          Our partnerships and memberships help connect students,
          faculty, and the college with the wider technology community.
        </p>
      </div>

      <div class="partnership-grid">

        <article
          v-for="item in partnerships"
          :key="item.name"
          class="partnership-card"
        >

          <div class="partnership-icon">
            ✓
          </div>

          <h3>{{ item.name }}</h3>

          <p>
            {{ item.description }}
          </p>

        </article>

      </div>

    </div>

  </section>
</template>