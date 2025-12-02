<template>
  <div class="padre">
    <MenuSuperior />
    <MenuInferior />
    <div class="contenedor">
      <CardComponente nombre="Lamborghini" kilometraje="1500" />
      <CardComponente nombre="Porsche" kilometraje="14500" />
      <CardComponente nombre="Ferrari" kilometraje="22000" />
      <CardComponente nombre="Toyota" kilometraje="5000" />
    </div>
  </div>


</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import CardComponente from './components/CardComponente.vue'
import MenuSuperior from './components/MenuSuperior.vue';
import MenuInferior from './components/MenuInferior.vue';

export default {
  name: 'App',
  components: {
    CardComponente,
    MenuSuperior,
    MenuInferior
    //HelloWorld
  }
}
</script>

<style>

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.contenedor {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 80%;
  margin: 2rem auto;
  gap: 20px;
  padding: 20px;
}
</style>
