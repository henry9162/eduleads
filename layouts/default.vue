<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
      temporary
    >
      <v-list>
        <v-list-item v-for="(item, i) in items" :key="i" :to="item.to" router exact>
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <div app class="py-md-5">
      <v-container>
        <v-app-bar-nav-icon class="d-sm-none" @click.stop="drawer = !drawer" />
        <div class="d-none d-sm-flex justify-space-between align-center">
          <v-toolbar-title v-text="title" />

          <ul class="d-none d-sm-flex flex-row justify-space-between align-center text-center">
            <li>Become a tutor</li>
            <li>Apply as tutor</li>
            <li>About us</li>
            <li>Contact us</li>
          </ul>

          <v-btn class="primary">Login</v-btn>
        </div>
        <v-spacer />
      </v-container>
    </div>

    <v-content>
      <!-- <v-container> -->
      <nuxt />
      <!-- </v-container> -->
    </v-content>

    <v-footer dark :fixed="fixed">
      <v-container>
        <v-row class="" dense>
          <v-col cols="12" :sm="3" class="d-flex flex-column">
            <p>EduLeads</p>
            <p class="caption">
              Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so.
              Click on the learn more button to get started.
            </p>
            <div>
              <span>&copy; {{ new Date().getFullYear() }}</span>
              <small>Terms and policy</small>
            </div>
          </v-col>
          <v-col cols="12" :sm="3" class="d-flex flex-column">
            <p>Links</p>
            <div class="links">
              <small class="subtitle d-block">About Us</small>
              <small class="subtitle d-block">Become a partner</small>
              <small class="subtitle d-block">Find a tutor</small>
            </div>
          </v-col>
          <v-col cols="12" :sm="3" class="d-flex flex-column">
            <p>Socials</p>
            <div class="links">
              <small class="subtitle d-block">Facebook</small>
              <small class="subtitle d-block">Instagram</small>
              <small class="subtitle d-block">Twitter</small>
            </div>
          </v-col>
          <v-col cols="12" :sm="3" class="d-flex flex-column">
            <p>Have any question?</p>
            <small class="font-weight-bold mb-3">
              If you have any questions you can
              reach us
            </small>
            <div class="links">
              <small class="subtitle d-block">0800000000</small>
              <small class="subtitle">email@domain.com</small>
              <small class="subtitle">Chat on Whatsapp</small>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/"
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire"
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Eduleads"
    };
  }
};
</script>

<style lang="scss" scoped>
ul {
  list-style: none;
  li {
    margin-left: 15px;
    margin-right: 15px;
  }
}
div.links > * {
  margin-bottom:5px;
}
</style>