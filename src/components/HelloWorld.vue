<template>
  <div class="hello">
    <p>🎸</p>
    <textarea v-model="tabs" class="tab-area" cols="100" rows="10">

    </textarea>
    <button @click="calculateSong">calc</button>
    <br />
    song: {{song}}
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      tabs: `e|-----0-------------------0-----0----------------0-------0-------------------3p0-------0---|
B|--3-----3--1-------1--------3-----3--1------1-----3--3----3--1-------1----1------1h3--1---|
G|--------------0h2--2--2----------------0h2----0-----------------0h2--2--2-----------------|
D|-------------------3-------------------------------------------------3--------------------|
A|--------------------------------------------0-----------------------------------------0---|
E|----------------------------3---------------------3--3---------------------------3--------|`,
      song: [],
    };
  },
  methods: {
    calculateSong: function () {
    },
  },
};
</script>🚲

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tab-area {
  border: 1px solid rgb(237, 237, 237);
  border-radius: 5px;
}
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
