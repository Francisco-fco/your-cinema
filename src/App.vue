<template>
  <div id="nav">
    <router-link to="/">HOME</router-link> |
    <router-link to="/about">COMING SOON</router-link>|
    <router-link to="/about">SIGN UP</router-link>|
    <router-link to="/about">GIFT CARDS</router-link>|
    <router-link to="/about">ABOUT</router-link>

    <!-- <div>
      <img src="./assets/breal.jpg" alt="">
    </div>
    -->
  </div>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 5%;
  background-color: rgb(253, 76, 76);
  
}

#nav a {
  font-weight: bold;
  color: #ffffff;
  text-decoration: none;
  padding-right: 0.3vw;
}

#nav a.router-link-exact-active {
  color: #050505;
  font-weight: bold;
}

/*div > img {
  width: 10%;
}
*/
</style>
