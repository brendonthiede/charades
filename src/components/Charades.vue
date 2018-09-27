<template>
  <div class="charades">
    <h1>Your word:</h1><h1>{{ msg }}</h1>
    <button id="new-word" v-on:click="GetNewWord">New Word</button>
  </div>
</template>

<script>
export default {
  name: "Charades",
  data: function() {
    return {
      msg: "Press 'New Word' to begin",
      wordList: [
        "Beauty and the Beast",
        "Bend It Like Beckham",
        "Charlotte's Web",
        "Chicken Run",
        "Cinderella",
        "Curious George",
        "Despicable Me",
        "Don't Tell Mom the Babysitter's Dead",
        "Ella Enchanted",
        "Finding Nemo",
        "Freaky Friday",
        "Ghostbusters",
        "Green Eggs and Ham",
        "Hairspray",
        "Hansel and Gretel",
        "Harry Potter",
        "High School Musical",
        "Holes",
        "Home Alone",
        "Howl's Moving Castle",
        "Inkheart",
        "Jack and the Beanstalk",
        "Little Red Riding Hood",
        "Madeline",
        "Mama Mia!",
        "Matilda",
        "Monsters, Inc.",
        "Mouse Hunt",
        "Mr Popper's Penguins",
        "Mrs. Doubtfire",
        "No, David!",
        "Pippi Longstocking",
        "Pirates of the Caribbean",
        "Rapunzel",
        "Rumpelstiltskin",
        "Shrek",
        "Sleeping Beauty",
        "Snow White",
        "Specky Magee",
        "Spy Kids",
        "The Frog Prince",
        "The Gingerbread Man",
        "The Giving Tree",
        "The Incredibles",
        "The Lion, The Witch and the Wardrobe",
        "The Lion, the Witch, and the Wardrobe",
        "The Little Mermaid",
        "The Lorax",
        "The Mummy",
        "The Nightmare Before Christmas",
        "The Pied Piper",
        "The Pink Panther",
        "The Polar Express",
        "The Princess Diaries",
        "The Secret Garden",
        "The Simpsons Movie",
        "The Three Little Pigs",
        "The Very Hungry Caterpillar",
        "The Wizard of Oz",
        "Thumbelina",
        "Tom Thumb",
        "Toy Story 3",
        "Up!",
        "Wall-E",
        "Where the Wild Things Are",
        "Where's Wally"
      ]
    };
  },
  methods: {
    GetNewWord: function() {
      this.msg = this.wordList[Math.floor(Math.random() * this.wordList.length)];
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  font-size: 200%
}
</style>
