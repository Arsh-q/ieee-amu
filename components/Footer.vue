<template>
  <v-card>
    <v-footer dark height="auto" class="footer pa-0">
      <v-card
        flat
        width="100%"
        tile
        class="dark lighten-1 white--text text-center"
      >
        <v-card-text>
          <v-btn
            v-for="social in socials"
            :key="social.icon"
            :href="social.link"
            target="_blank"
            rel="noopener"
            class="mx-4"
            dark
            icon
          >
            <v-icon size="24px">{{ social.icon }} </v-icon>
          </v-btn>
        </v-card-text>
        <v-card-text class="white--text pt-0">
          <strong>
            Zakir Husain College of Engineering and Technology, Aligarh Muslim
            University, Aligarh, Uttar Pradesh, India</strong
          >
        </v-card-text>
        <v-card-text class="white--text pt-0 pb-0">
          <v-btn
            text
            href="https://github.com/ieee-amu/ieee-amu/graphs/contributors"
            target="_blank"
            rel="noopener"
          >
            <span class="developers"
              >made with <v-icon class="developers">mdi-heart</v-icon> by
              db</span
            >
          </v-btn>
        </v-card-text>
        <v-card-text class="white--text">
          &copy; {{ new Date().getFullYear() }} — <strong>IEEE AMU</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    socials: [
      { icon: 'mdi-facebook', link: 'https://facebook.com/AMUIEEE' },
      { icon: 'mdi-github', link: 'https://github.com/ieee-amu' },
      { icon: 'mdi-instagram', link: 'https://instagram.com/ieeeamu' },
      {
        icon: 'mdi-linkedin',
        link: 'https://www.linkedin.com/company/ieee-amu-student-branch/',
      },
    ],
  }),
}
</script>
