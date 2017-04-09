<template>
  <div class="shelfy">
    <input v-model="title" placeholder="Add a game">
    <button v-on:click="addGame(games, title)">Add</button>
    <ul>
      <li v-for="game in games">
        {{game.name}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'shelfy',
  data () {
    return {
      games: []
    }
  },
  methods: {
    addGame: function (games, title) {
      const item = {name: title}
      games.push(item)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
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
