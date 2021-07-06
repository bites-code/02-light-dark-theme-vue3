<template>
  <div :class="theme === 'light' ? 'light-theme' : 'dark-theme'" class="main-body">
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
      theme: "light"
    }
  },
  methods: {
    changeTheme() {
      console.log("I am changing theme");
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
.light-theme {
  background-color: white;
  color: black;
}
.dark-theme {
  background-color: black;
  color: white;
}
</style>