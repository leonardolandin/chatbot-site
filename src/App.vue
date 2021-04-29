<template>
  <div id="app">
  </div>
</template>

<script>

export default {
  name: 'App',
    mounted() {
      window.watsonAssistantChatOptions = {
      integrationID: "be8292de-ed89-4a68-a232-1b97601115c5", // The ID of this integration.
      region: "us-south", // The region your integration is hosted in.
      serviceInstanceID: "4f423d71-0d8c-4d5b-be01-74361880bb98", // The ID of your service instance.
      onLoad: function(instance) { instance.render(); }
    }
    setTimeout(function() {
      const t = document.createElement('script');
      t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
      document.head.appendChild(t);
    })
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
  margin: 0;
  overflow-x: hidden;
  overflow-y: hidden;
}
</style>
