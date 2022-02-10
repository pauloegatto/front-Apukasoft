<template>
  <div>
    <!-- -----------------------------------------------
          Start Header
    ----------------------------------------------- -->
    <v-app-bar
      app
      class="app-header position-relative bg-dark header1"
      flat
    >
      <v-container class="py-0 fill-height">
        <!-- Logo -->
        <div class="logo">
          <NLink to="/">
            <v-img
              :src="require('@/assets/images/logos/apuka-logo.png')"
              alt="logo"
            />
          </NLink>
        </div>

        <v-spacer></v-spacer>
        <v-btn class="d-block d-md-none" text @click="toggleClass()">
          <v-app-bar-nav-icon />
        </v-btn>
        <!-- Desktop view Navigation -->
        <div
          class="navigation"
          v-bind:class="[isActive ? 'd-block' : '']"
          @click="isActive = !isActive"
        >
          <ul class="navbar-nav">
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="/"> Inicio </n-link>
            </li>
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="/">Cartão CCB</n-link>
            </li>
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="/">Contato</n-link>
            </li>
            
          </ul>
        </div>
        <!-- login-regiter -->
       
      </v-container>
    </v-app-bar>
    <!-- -----------------------------------------------
          End Header
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "Header1",
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggleClass: function (event) {
      this.isActive = !this.isActive;
    },
  },
};
</script>
