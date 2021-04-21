<template>
  <div id="app">
    <Chat />
  </div>
</template>

<script>
import Chat from './components/Chat.vue'

export default {
  name: 'App',
  components: {
    Chat
  }
}
</script>

<style>
#app {
    display: flex;
    width: 100vw;
    height: 100vh;
    justify-content: center;
    align-items: center;
    background: linear-gradient(45deg,rgba(1,100,152,.92),rgba(14,113,197,.68));
}

body {
  margin: 0
}
</style>
