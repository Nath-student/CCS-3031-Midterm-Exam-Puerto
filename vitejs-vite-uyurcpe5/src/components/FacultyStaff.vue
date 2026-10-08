<script setup>
const faculty = [
  {
    position: 'Dean',
    name: 'Dr. Faculty Name',
    education: 'PhD in Information Technology',
    image: 'https://i.pravatar.cc/300?img=12'
  },

  {
    position: 'Program Chair - BSIT',
    name: 'Prof. Faculty Name',
    education: 'Master of Information Technology',
    image: 'https://i.pravatar.cc/300?img=32'
  },

  {
    position: 'Program Chair - BSCS',
    name: 'Prof. Faculty Name',
    education: 'Master of Computer Science',
    image: 'https://i.pravatar.cc/300?img=47'
  },

  {
    position: 'Faculty Member',
    name: 'Prof. Faculty Name',
    education: 'Master of Information Systems',
    image: 'https://i.pravatar.cc/300?img=49'
  },

  {
    position: 'Faculty Member',
    name: 'Prof. Faculty Name',
    education: 'Master of Library and Information Science',
    image: 'https://i.pravatar.cc/300?img=44'
  },

  {
    position: 'Staff',
    name: 'Staff Name',
    education: 'Bachelor of Information Technology',
    image: 'https://i.pravatar.cc/300?img=5'
  }
]
</script>

<template>
  <section id="faculty" class="section faculty-section">

    <div class="container">

      <div class="section-heading">
        <p class="eyebrow">OUR PEOPLE</p>

        <h2>Faculty & Staff</h2>

        <p>
          Meet the faculty and staff who support the academic
          development and success of our students.
        </p>
      </div>

      <div class="org-chart">

        <div class="org-level">
          <div class="org-position">
            <strong>College Dean</strong>
            <span>College Leadership</span>
          </div>
        </div>

        <div class="org-line"></div>

        <div class="org-level">

          <div class="org-position">
            <strong>BSIT</strong>
            <span>Program Team</span>
          </div>

          <div class="org-position">
            <strong>BSCS</strong>
            <span>Program Team</span>
          </div>

          <div class="org-position">
            <strong>BSDMIA</strong>
            <span>Program Team</span>
          </div>

          <div class="org-position">
            <strong>BLIS</strong>
            <span>Program Team</span>
          </div>

        </div>

      </div>

      <div class="faculty-grid">

        <article
          v-for="person in faculty"
          :key="person.position + person.name"
          class="faculty-card"
        >

          <img
            :src="person.image"
            :alt="person.name"
          />

          <div class="faculty-info">

            <span class="faculty-position">
              {{ person.position }}
            </span>

            <h3>{{ person.name }}</h3>

            <p>
              {{ person.education }}
            </p>

          </div>

        </article>

      </div>

    </div>

  </section>
</template>