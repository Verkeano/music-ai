<template>
  <div class="App">
    <header class="App-header">
      <h1>LyricAI</h1>
      <h6>Search with lyrics</h6>
    </header>
    <div class="form">
      <textarea :value="Lyrics" @input="updateLyrics" class="search-for-lyrics" cols="30" rows="10"></textarea>
      <button type="submit">Search</button>
    </div>
    <h6>{{ Lyrics }}</h6>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      Lyrics: "",
    };
  },
  methods: {
    updateLyrics(event) {
      this.Lyrics = event.target.value;
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
.App {
  text-align: center;
}

.App-header {
  background-color: #282c34;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
  color: white;
}
textarea {
  width: 50%;
  margin-left: auto;
  margin-right: auto;
  height: auto;
  max-height: 50%;
  resize: none;
}

.form {
  display: flex;
  flex-direction: column;
  align-items: center;
  left: 50%;
  top: 50%;
}
</style>
