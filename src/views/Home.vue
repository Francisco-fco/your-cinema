<template>
  <div class="home">
    <img class="image" src="../assets/once-upon-a-time.png" />
    <div id="description">
      <HomeComponent
        title="ONCE UPON A TIME IN HOLLYWOOD"
        text="A faded television actor and his stunt double strive to achieve fame and
        success in the final years of Hollywood's Golden Age in 1969 Los
        Angeles."
        style="color: white"
      />
    </div>
  </div>
  <section class="homepage">
    <div class="mini-nav">
      <button><h5>By Day</h5></button>
      <button><h5>By Movie</h5></button>
      <button><h5>Print</h5></button>
      <button><h5>Latest First</h5></button>
    </div>
    <div class="calendar-red">
      <input type="date" />
    </div>
    <div class="movie">
      <img src="../assets/ladybird.png" alt="" />
      <p>
        Lady Bird is a 2017 American coming-of-age comedy-drama film written and
        directed by Greta Gerwig in her solo directorial debut. Set between 2002
        and 2003 in Sacramento, California, it is a coming-of-age story of a
        high school senior and her strained relationship with her mother, family
        members and friends.
      </p>
      <div id="trailer">
        <button>Watch trailer</button>
      </div>
    </div>
    <div class="movie">
      <img src="../assets/tenet.jpg" alt="" />
      <p>
        This is a science fiction-action-thriller film starring John David
        Washington, Robert Pattinson, Elizabeth Debicki, and Kenneth Branagh,
        among others. It's the story of a secret agent who learns to manipulate
        the flow of time to prevent an attack from the future that threatens to
        annihilate the present.
      </p>
      <div id="trailer">
        <button>Watch trailer</button>
      </div>
    </div>
    <div class="movie">
      <img src="../assets/judy.png" alt="" />
      <p>
        Judy is a 2019 biographical drama film based on the life of American
        actress Judy Garland. Directed by Rupert Goold, it is an adaptation of
        the Olivier- and Tony-nominated West End and Broadway play End of the
        Rainbow by Peter Quilter.
      </p>
      <div id="trailer">
        <button>Watch trailer</button>
      </div>
    </div>
    <div class="movie">
      <img src="../assets/wonderwoman.png" alt="" />
      <div id="text">
        <p>
          In Wonder Woman, the Amazon princess Diana sets out to stop World War
          I, believing the conflict was started by the longtime enemy of the
          Amazons, Ares, after American pilot and spy Steve Trevor crash-lands
          on their island Themyscira and informs her about it.
        </p>
      </div>
      <div id="trailer">
        <button>Watch trailer</button>
      </div>
    </div>
  </section>
  <footer>
    <div class="footer">
      <h5>&copy;Copyright</h5>
    </div>
  </footer>
</template>

<script>
// @ is an alias to /src
import HomeComponent from "@/components/HomeComponent.vue";

export default {
  name: "Home",
  components: {
    HomeComponent,
  },
};
</script>

<style>
.home {
  position: relative;
  background-color: rgb(41, 41, 41);
  width: 100%;
  display: flex;
  justify-content: center;
}

.image {
  width: 87%;
  margin: 0%;
  padding: 0%;
}

#description {
  width: 100%;
  position: absolute;
  bottom: 0;
}

.homepage {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 20vw;
  margin-top: 2vw;
  background-color: whitesmoke;
}

.mini-nav {
  display: flex;
  justify-content: space-between;

  background-color: rgb(29, 29, 29);
  padding: 1vw;
}

.mini-nav > button {
  color: white;
  background-color: rgb(0, 0, 0);
  font-size: 1.7vw;
  padding-right: 2vw;
  padding-left: 2vw;
  padding-top: 0;
  border-radius: 15%;
}

.mini-nav > button > h5 {
  margin: 0;
  padding: 0;
  padding-top: 0.3vw;
  padding-bottom: 0.3vw;
}

.calendar-red {
  display: flex;
  justify-content: center;
  background-color: rgb(253, 76, 76);
  padding: 2vw;
}

.movie {
  position: relative;
  display: flex;
  padding: 2vw;
}

.movie > img {
  width: 22vw;
  height: 22vh;
}

.movie > p {
  padding-top: 2vw;
  padding-left: 0.8vw;
  padding-right: 15vw;
  padding-bottom: 2vh;
}

#text{
  display: flex;
  

}
#trailer {
  display: flex;
  flex-direction: column;
  margin: 0;
  padding: 0;
}

#trailer > button {
  position: absolute;
  bottom: 2vh;
  right: 27vw;
  color: white;
  background-color: rgb(253, 76, 76);
  border: none;
  padding-left: 1vw;
  padding-right: 1vw;
  padding-top: 0.3vw;
  padding-bottom: 0.3vw;
}

.footer {
  color: white;
  background-color: black;
  padding: 1vw;
}
</style>
