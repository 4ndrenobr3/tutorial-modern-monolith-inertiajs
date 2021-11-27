<template>
  <h1>Users</h1>
  <Nav />
  <div style="margin-top: 800px">
      <p>The current time is {{ time }}</p>
  </div>

  <Link
    href="/users" 
    class="text-blue-500"
    preserve-scroll
    >
    Refresh
  </Link>
</template>

<script>
import Nav from '../Shared/Nav.vue'
import { Link } from '@inertiajs/inertia-vue3'

export default {
  props: { time: String },
  components: { Nav, Link }
}
</script>

<style>

</style>