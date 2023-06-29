<template>
  <div id="app">
    <h1>Nama : {{namaLengkap}}</h1>
    <h1>Asal Sekolah : {{asal}}</h1>
    <h1>kelas : {{kelas}}</h1>
    <h1>umur : {{umur}}</h1>
    <button @click='add()'>Click here</button>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nama : "Ghazwan Krisna Fauzan",
      asal : "SMK Assalaam Bandung",
      kelas : "X Rpl 1",
      umur : "20 Tahun",
    };
  },
  computed: {
    namaLengkap() {
      return this.nama + " Syncl";
    }
  },
  methods : {
    add() {
      this.nama = "Ghaz";
      console.log("AHAHAHAH")
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
