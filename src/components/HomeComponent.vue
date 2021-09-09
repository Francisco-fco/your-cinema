<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <h5>{{ text }}</h5>
    <div class="button-desc">
      <button style="background-color: rgba(0, 0, 0, 0.644)">
        <h5>Watch now!</h5>
      </button>
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

h3 {
  margin: 40px 0 0;
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

.button-desc > button > h5 {
  color: white;
  padding: 0.2vw;
  margin: 0;
}
</style>
