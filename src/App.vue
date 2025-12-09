<template>
  <div class="padre">
    <MenuSuperior />
    <MenuInferior />
    <!-- <MainComponent /> -->
    <div class="contenedor">
      <div v-for="carro in carros" :key="carro.id">
        <CardComponente 
            :nombre="carro.nombre" 
            :kilometraje="carro.kilometraje"
            :imagen="carro.imagen" />
      </div>
    </div>
  </div>


</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import CardComponente from './components/CardComponente.vue'
import MenuSuperior from './components/MenuSuperior.vue';
import MenuInferior from './components/MenuInferior.vue';
// import MainComponent from './components/MainComponent.vue';

export default {
  name: 'App',
  data(){
    return{
      carros: [
        {id: 1, nombre: 'Lamborghini', kilometraje: 1500, imagen: "lamborghini.jpg"},
        {id: 2, nombre: 'Porsche', kilometraje: 14500, imagen: 'porsche.jpg'},
        {id: 3, nombre: 'Ferrari', kilometraje: 22000, imagen: 'ferrari.jpeg'},
        {id: 4, nombre: 'Toyota', kilometraje: 5000, imagen: 'Toyota-corolla.png'},
        {id: 5, nombre: 'Chevrolert', kilometraje: 75000, imagen: 'Chevrolet.png'},
         {id: 6, nombre: 'KIA', kilometraje: 0, imagen: 'kia.png'},
      ]
    }
  },
  components: {
    CardComponente,
    MenuSuperior,
    MenuInferior,
    // MainComponent
    //HelloWorld
  },
  methods: {
    imprimirCarros(){

      for(let carro of this.carros){
        console.log(`El carro ${carro.nombre} tiene un kilometraje de ${carro.kilometraje} km.`);
      }

    }
  },

  created(){
    this.imprimirCarros();
    
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
