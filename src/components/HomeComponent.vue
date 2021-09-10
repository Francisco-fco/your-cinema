<template>
  <div class="hello">
    <div id="title">
      <h1>{{ title }}</h1>
    </div>
    <div id="text">
      <h5>{{ text }}</h5>
    </div>
    <div class="button-desc">
      <div id="trailer-nav">
        <a href="https://www.youtube.com/watch?v=ELeMaP8EPAA&t=42s"
          ><button>Watch trailer</button></a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeComponent",
  props: {
    title: String,
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  background-color: rgba(0, 0, 0, 0.616);
  padding: 0.1vw;
}

#trailer-nav {
  display: flex;
  position: relative;
}

#trailer-nav > a > button {
  width: 10vw;
  height: 4vh;
  position: absolute;
  bottom: 5.6vh;
  left: 70vw;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}

.button-desc {
  margin: 0;
  padding: 0;
}
</style>
