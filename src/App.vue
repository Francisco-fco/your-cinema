<template>
  <div id="nav">
    <img src="./assets/logo.png" />
    <div id="routes">
      <router-link to="/">HOME</router-link> |
      <router-link to="/about">COMING SOON</router-link>|
      <router-link to="/sign-up">SIGN UP</router-link>|
      <router-link to="/about">GIFT CARDS</router-link>|
      <router-link to="/about">ABOUT</router-link>
    </div>

    <!-- <div>
      <img src="./assets/breal.jpg" alt="">
    </div>
    -->
    <div id="socialmedia">
      <img src="./assets/Facebook60x60.png" />
      <img src="./assets/Instagram60x60.png" />
      <img src="./assets/Twitter60x60.png" />
      <img src="./assets/YouTube60x60.png" />
    </div>
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
  position: relative;
  display: flex;
  justify-content: space-between;
  padding: 5%;
  background-color: rgb(253, 76, 76);
}

#nav > #routes {
  position: absolute;
  left: 65vw;
  top: 19vh;
}

#nav > #routes > a {
  font-weight: bold;
  color: #ffffff;
  text-decoration: none;
  width: 100%;
  padding-right: 1vw;
  padding-left: 1vw;
}

#nav a.router-link-exact-active {
  color: #050505;
  font-weight: bold;
}

#nav > #socialmedia {
  position: absolute;
  top: 8vh;
  left: 75vw;
}

/*div > img {
  width: 10%;
}
*/
</style>
