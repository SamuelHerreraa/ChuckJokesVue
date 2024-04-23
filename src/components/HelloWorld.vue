<template>
  <div id="app">
    <h1>Chuck Norris Jokes</h1>
    <ul>
      <li v-for="joke in chuck" :key="joke.value">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      chuck: [ 
        { "value": "Chuck Norris can skydive into outer space." },
        { "value": "The chief export of Chuck Norris is pain." },
        { "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { "value": "Time waits for no man. Unless that man is Chuck Norris." },
        { "value": "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ]
    }
  }
}
</script>

<style>
#app {
  text-align: center;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  padding: 8px;
  margin: 5px;
  background-color: #f0f0f0;
  border-radius: 8px;
}
</style>
