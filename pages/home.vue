<template>
  <div>
    <h1>Login Success</h1>
    <p>User Name: {{this.$auth.$state.user.name}}</p>
    <button @click="logout">Logout</button>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component({})
export default class Logout extends Vue {
  logout() {
    this.$auth.logout();
  }
}
</script>
