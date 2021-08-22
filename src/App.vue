<template>
  <StatsPreviewComponent/>
</template>

<script>
import StatsPreviewComponent from './components/StatsPreviewComponent.vue'

export default {
  name: 'App',
  components: {
    StatsPreviewComponent
  }
}
</script>

<style>

:root {
  --very-dark-blue: hsl(233, 47%, 7%);
  --dark-blue: hsl(244, 38%, 16%);
  --purple: hsl(277, 64%, 61%);
  --white: hsl(0, 0%, 100%);
  --transparent-white: hsla(0, 0%, 100%, 0.75);
  --very-transparent-white: hsla(0, 0%, 100%, 0.6);
}

html {
  font-size: 62.5%;
}

body {
  background-color: var(--very-dark-blue);
  width: 100vw;
  height: 100vh;
  overflow: hidden;
}


#app {
  font-family: 'Inter', 'Lexend Deca', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: var(--white);
}

</style>
