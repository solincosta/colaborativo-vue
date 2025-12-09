<template>
  <div class="card">
    <img class="image" :src="require(`@/assets/${imagen}`)" alt="">
    <h3>{{ nombre }}</h3>
    <h5>{{ kilometraje }}</h5>
    <span v-if="kilometraje == 0" class="estado-nuevo">NUEVO</span>
    <span v-else class="estado-usado">USADO</span>
  </div>
</template>

<script>
export default {
  name: 'CardComponente',

  props: {
    nombre: String,
    kilometraje: Number,
    imagen: String
  }
}
</script>

<style scope>
.card {
  height: 300px;
  width: 200px;
  border: 1px solid black;
  border-radius: 10px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3);
  display: flex;
  flex-direction: column;
}

.image {
  height: 70%;
  width: 100%;
}

h3 {
  text-align: center;
  margin: 0;
  padding: 10px 0;
  height: 15%;
}

h5 {
  text-align: center;
  margin: 0;
  padding: 10px 0;
  height: 15%;
}

.estado-nuevo {
  background-color: green;
  color: white;
  padding: 3px;
  width: fit-content;
  border-radius: 5px;
  text-align: center;
  font-size: 12px;
}

.estado-usado {
  background-color: gray;
  color: white;
  padding: 3px;
  width: fit-content;
  border-radius: 5px;
  text-align: center;
  font-size: 12px;
}
</style>