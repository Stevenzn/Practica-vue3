<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo" width="125" height="125" />
    <small>
      <h1>ContadorApp</h1>
    </small>
    <hr />
    <h2>contador: {{ contador }}</h2>
    <button @click="sumar()">+1</button>
    <button @click="restar()">-1</button>
    <button @click="reset()">reset</button>
  </div>
</template>

<script>
export default {
  data: ()=> ({
      contador: 0,
  }),
  methods: {
    sumar(){
      this.contador++;
    },
    restar(){
      this.contador--;
    },
    reset(){
      this.contador = 0;
    }
},
};
</script>

<style scoped>
.container {
  text-align: center;
}
small {
  color: #666;
}

h1 {
  font-weight: bolder;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 2rem;
  margin: 0px 10px;
}
</style>
