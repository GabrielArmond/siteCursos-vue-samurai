<template>
  <div class="home">
    <b-container>
      <b-row align-v="center">
        <Card v-for="curso in cursos" :key="curso.id" :nome="curso.nome" />
      </b-row>
    </b-container>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/Card.vue'

export default {
  name: 'Home',

  data() {
    return {
      cursos: []
    }
  },

  components: {
    Card
  },

  mounted() {
    this.fetchData()
  },

  methods: {
     async fetchData(){
      try{
        const response = await fetch('cursos.json');
        const val = await response.json();
        this.cursos = val;
        console.log(this.cursos);
      }catch(err){
        console.log(err);
      }
  }
  }
}
</script>
