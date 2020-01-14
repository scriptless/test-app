<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default class HelloWorld extends Vue {

  test() {
    const city = "berlin";
    const element = document.getElementById(city);
    if(element == null) return;
    const offset = element.getBoundingClientRect().top - 250;

    window.scrollTo({
        top: offset,
         behavior: "smooth"
     });
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
a {
  color: #42b983;
}
</style>
