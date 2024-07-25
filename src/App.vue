<template>
  <main>
    <main>
    <body>
      <div className="App">
        <header class="App-header">
          <h1>LyricAI</h1>
          <h6>Search with lyrics</h6>
        </header>	
        <header class="form">
          <textarea bind:value={Lyrics}  class="search-for-lyrics" cols="30" rows="10" type="text"/>
          <button type="submit">Search</button>
        </header>
        <h6>{Lyrics}</h6>
      </div>
    </body>
    </main>
  </main>
</template>

<script>
let Lyrics = "";
export default {
  name: 'App',
}
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
