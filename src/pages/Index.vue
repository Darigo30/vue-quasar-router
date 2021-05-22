<template>
  <q-page class="flex flex-center">
    <div class="row">
      <div class="col-4" v-for="(mostrarimagen, iund) in personajes" :key="iund">
        <q-card class="my-card">
          <img v-bind:src="mostrarimagen.imagen">
          <q-card-section>
            <div class="text-h6">{{ mostrarimagen.nombre}}</div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'Index',
  data() {
    return {
      personajes: [
       {
         id: "1",
         nombre: "Morty",
         imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
       },
       {
         id: "2",
         nombre: "Rick",
         imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
       },
       {
         id: "3",
         nombre: "Summer",
         imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
       },
       {
         id: "4",
         nombre: "Beth",
         imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
       },
       {
         id: "5",
         nombre: "Jerry",
         imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
       },
      ]
    };
  },
}
</script>
<style scoped>
  
  .col-4{
    padding: 15px;
  }
  
</style>
