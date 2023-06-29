<template>
  <div id="app">
    <div>
      {{ massage }}
    </div>
    <button @click='add()'>Hai</button>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      massage: 'hai',
    };
  },
  methods : {
    add : () => {
      alert('hai')
      console.log("HAI")
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
