<template>
  <div class="containerChat">
    <div>
      <div class="containerName">
        <input type="text" placeholder="Nome de usuário">
      </div>

      <div class="containerChatMessages">
      </div>

      <div class="containerMessage">
        <textarea name="" id="" cols="30" rows="10"></textarea>
      </div>

      <div class="containerSend">
        <button>Enviar</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.containerChat {
  width: 30%;
  flex-direction: column;
  display: flex;
  background-color: white;
  padding: 40px;
}

input {
  width: 50%;
  height: 30px;
  border-radius: 8px;
  border: 2px solid gray;
  outline: none;
  padding: 10px;
}

.containerChatMessages {
  margin-top: 30px;
  height: 390px;
  border-radius: 8px;
  border: 2px solid gray;
}

.containerMessage {
  margin-top: 40px;
}

.containerMessage > textarea {
  border-radius: 8px;
  min-height: 84px;
  min-width: 99%;
  max-height: 84px;
  max-width: 99%;
  border: 2px solid gray;
}

.containerSend {
  margin-top: 40px;
}

.containerSend > button {
  outline: none;
  background: #4285f4;
  width: 100%;
  border: 0;
  border-radius: 4px;
  padding: 12px 20px;
  color: #fff;
  font-family: inherit;
  font-size: inherit;
  font-weight: 500;
  line-height: inherit;
  text-transform: uppercase;
  cursor: pointer;
}
</style>
