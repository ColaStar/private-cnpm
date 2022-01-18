<template>
  <div id="app">
    <img src="./assets/logo.png" />
    <h1>{{ msg }}</h1>
    <h2>章三的包</h2>
    <Main :propData="initData" />
  </div>
</template>

<script>
import Main from "./components/Main";

export default {
  name: "app",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      initData: "hello 你好",
    };
  },
  components: {
    Main,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
