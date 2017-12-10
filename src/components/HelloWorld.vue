<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <svg class="svgclass">
      <circle class="svgcircle" cx="100" cy="100" r="30" @click="circlk"></circle>
      <text class="svgtext" x="150" y="120">I can do this!!!</text>
      <path class="svgpath" d="M 150,150 L 1000,150"></path>
    </svg>
    <img src="../assets/MIP.svg"></img>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    circlk (evt) {
      alert('circle click!')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-weight: normal;
}
.svgclass {
  border: 2px solid black;
  height: 200px;
  width: 1000px;

}
.svgcircle {
  fill: red;
  stroke: green;
}
.svgtext {
  font-size: 40px;
  font-family: sans-serif;
  font-weight: bold;
  fill: purple;
  stroke: yellow;
}

.svgpath {
  fill: blue;
  stroke: green;
  stroke-width: 5px;

}
</style>
