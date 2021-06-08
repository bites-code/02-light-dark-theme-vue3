<template>
  <div :class="theme === 'light' ? 'body-light' : 'body-dark'" class="main-body">
    <div class="flex">
      <div>Theme selection in Vue 3</div>
      <div></div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      theme: "dark"
    }
  }
}
</script>

<style>
.main-body {
  height: 100vh;
  padding: 0 2px 0 2px;
}
.body-light {
  background-color: white;
  color: black;
}
.body-dark {
  background-color: black;
  color: white;
}
.flex {
  display: flex;
}
</style>