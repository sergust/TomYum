<template>
  <v-container class="grey cont elevation-5">
    <v-row class="header elevation-15 justify-center">
      <v-col cols="2">
        <img src="../../assets/logo.svg" alt="Tom Yum" class="logo" />
      </v-col>
      <v-col cols="2">
        <app-header-auth></app-header-auth>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import HeaderAuth from './HeaderAuth.vue';
export default {
  data() {
    return {
      username: 'Username'
    };
  },
  components: {
    appHeaderAuth: HeaderAuth
  }
};
</script>

<style>
.cont {
  background-color: grey;
  margin: 0;
  padding: 0;
  border-bottom-left-radius: 15px;
  border-bottom-right-radius: 15px;
}

.logo {
  width: 64px;
  height: 64px;
}
</style>
