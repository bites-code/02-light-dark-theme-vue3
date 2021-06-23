<template>
  <div :class="theme === 'light' ? 'body-light' : 'body-dark'" class="main-body">
    <div style="padding:5px">      
      <div>Theme selection in Vue 3</div>
      <button @click="changeTheme">Switch Theme</button>
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
  },
  methods: {
    changeTheme() {
      console.log("here");
      this.theme = this.theme === "dark" ? "light" : "dark";
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
</style>