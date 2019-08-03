<template>
  <div>
    <h1>Login Page</h1>
    <button @click="authenticate">Login</button>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
@Component({})
export default class Index extends Vue {
  authenticate() {
    this.$auth.loginWith('auth0')
  }
}
</script>
