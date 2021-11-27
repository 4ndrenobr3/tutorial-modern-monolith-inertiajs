<template>
  <nav class="mt-6">
    <ul class="list-disc">
      <li>
        <NavLink
          href="/"
          class="text-blue-500 hover:underline"
          :active="$page.component === 'Home'"
        >
          Home
        </NavLink>
      </li>
      <li>
        <NavLink
          href="/users"
          class="text-blue-500 hover:underline"
          :active="$page.component === 'Users'"
          >Users</NavLink
        >
      </li>
      <li>
        <NavLink
          href="/settings"
          class="text-blue-500 hover:underline"
          :active="$page.component === 'Settings'"
          >Settings</NavLink
        >
      </li>
      <li>
        <NavLink
          href="/logout"
          method="post"
          :data="{ foo: 'bar' }"
          as="button"
          class="text-blue-500 hover:underline"
          >Log out</NavLink
        >
      </li>
    </ul>
  </nav>
</template>

<script>
import NavLink from "../Shared/NavLink.vue";

export default {
  components: { NavLink },
};
</script>

<style>
</style>