<template src="./HomePage.html"></template>

<script>
export default {
  name: "home-page",
  data() {
    return {
        username: "Marley",
        MostPlayedChampions: [
            {Name: "Jinx", GamesPlayed: "567"},
            {Name: "Caitlyn", GamesPlayed: "250"},
            {Name: "Ashe", GamesPlayed: "60"},
            {Name: "Powder", GamesPlayed: "30"},
            {Name: "Jax", GamesPlayed: "2"}],
    }
  },
  methods: {
      btnSearch(){
          this.username = "Joey";
      },
  }
};
</script>

