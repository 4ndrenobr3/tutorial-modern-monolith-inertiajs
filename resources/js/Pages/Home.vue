<template>
  <h1>Hello World, {{ name }}</h1>
  <p>In this series, we will use the following frameworks:</p>
  <ul>
    <li v-for="(framework, key) of frameworks" :key="key" v-text="framework"></li>
  </ul>
</template>

<script>
export default {
    props: {
        name: String,
        frameworks: Array,
    }
}
</script>

<style>

</style>