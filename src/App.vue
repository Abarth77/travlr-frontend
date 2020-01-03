<template>
  <div id="app">
    <settings />
    <display />
  </div>
</template>

<script>
import Settings from '@/components/Settings';
import Display from '@/components/Display';

export default {
  name: 'app',
  components: { Settings, Display }
}
</script>

<style>
* {
  box-sizing: border-box;
}

html, body, #app {
  width: 100%;
  height: 100%;
  padding: 0;
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  width: 100%;
  height: 100%;
}
</style>
