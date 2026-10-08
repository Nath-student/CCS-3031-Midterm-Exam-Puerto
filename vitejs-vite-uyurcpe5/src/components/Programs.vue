<script setup>
const programs = [
  {
    code: 'BSIT',
    name: 'Bachelor of Science in Information Technology',
    description:
      'Focuses on developing skills in software development, web technologies, networking, database systems, and information technology management.',
    skills: [
      'Web Development',
      'Programming',
      'Database Management',
      'Networking'
    ]
  },

  {
    code: 'BSCS',
    name: 'Bachelor of Science in Computer Science',
    description:
      'Provides students with a strong foundation in computing, algorithms, programming, software development, and problem solving.',
    skills: [
      'Programming',
      'Algorithms',
      'Software Development',
      'Artificial Intelligence'
    ]
  },

  {
    code: 'BSDMIA',
    name: 'Bachelor of Science in Data Management and Information Analytics',
    description:
      'Prepares students to manage data and transform information into useful insights that support organizational decision-making.',
    skills: [
      'Data Management',
      'Data Analytics',
      'Information Systems',
      'Data Visualization'
    ]
  },

  {
    code: 'BLIS',
    name: 'Bachelor of Library and Information Science',
    description:
      'Combines information management, technology, research, and library science to prepare students for modern information environments.',
    skills: [
      'Information Management',
      'Digital Libraries',
      'Research',
      'Information Technology'
    ]
  }
]
</script>

<template>
  <section id="programs" class="section">
    <div class="container">

      <div class="section-heading">
        <p class="eyebrow">ACADEMIC PROGRAMS</p>

        <h2>Programs We Offer</h2>

        <p>
          Explore the programs offered by the College of Computer Studies.
        </p>
      </div>

      <div class="program-grid">

        <article
          v-for="program in programs"
          :key="program.code"
          class="program-card"
        >

          <div class="program-code">
            {{ program.code }}
          </div>

          <h3>{{ program.name }}</h3>

          <p>
            {{ program.description }}
          </p>

          <h4>Key Areas</h4>

          <ul>
            <li
              v-for="skill in program.skills"
              :key="skill"
            >
              {{ skill }}
            </li>
          </ul>

        </article>

      </div>
    </div>
  </section>
</template>