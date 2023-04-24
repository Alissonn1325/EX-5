<script setup>
import { ref }from 'vue'

const cidades = ref ([
    'São Paulo',
    'Rio de Janeiro',
    'Belo Horizonte',
    'Salvador',
    'Fortaleza',
    'Curitiba',
    'Manaus',
    'Recife',
    'Porto Alegre',
    'Brasília'
]
)
</script>

<template>
  <div class="tema">
   <ul>
    <h1>Cidades Gamers</h1>
    <hr>
    <li v-for="(cidade, index) in cidades.sort()" :key="index">{{ cidade }}</li>
  </ul>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bruno+Ace+SC&display=swap');
.tema {
  background-color: rgb(0, 0, 0);
  padding: 20px 30px;
  color: rgb(183, 210, 219);
  border-radius: 10px;
  text-align: center;
  display: flex;
  flex-direction: column;
  width: 28%;
  margin: 0 auto;
  margin-top: 12%;
  margin-bottom: 20px;
}

h1 {
  color: white;
  font-weight: bold;
  font-size: 1.5em;
  font-family: 'Bruno Ace SC', cursive;
}

li {
  margin: 15px 15px 15px 15px;
  color: white;
  font-family: 'Bruno Ace SC', cursive;
}
</style>
