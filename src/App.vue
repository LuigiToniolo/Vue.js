<template>

  <div>
    <h1>{{ titulo }}</h1>

    <ul>

      <li v-for="foto of fotos">
        <img :src="foto.url" :alt="foto.titulo">
      </li>

    </ul>

  </div>
</template>


<script>
export default {

  data() {
    return {

        titulo: 'Alurapic',
        fotos: [
          {
            url: 'https://carroscomcamanzi.com.br/wp-content/uploads/2019/12/Lamborghini-Lambo-Gran-Turismo-Concept-2019-1-1333x1000.jpg',
            titulo: 'carro'
          },
          {
            url: 'https://carroscomcamanzi.com.br/wp-content/uploads/2019/12/Lamborghini-Lambo-Gran-Turismo-Concept-2019-1-1333x1000.jpg',
            titulo: 'lambo'
          }
        ]
    }
  }
}

</script>

<style>
</style>
