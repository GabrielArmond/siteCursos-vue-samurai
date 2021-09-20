<template>
  <div>
    <b-col>
      <b-card
        :title="nome"
        img-src="https://picsum.photos/600/300"
        img-alt="Cursos"
        style="max-width: 20rem;"
        img-top
        tag="article"
        class="mb-2"
        border-variant="primary"
        header="Cursos de Programação"
        header-bg-variant="primary"
        header-text-variant="white"
        align="center"
      >
        <b-card-text>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolor esse
          totam fuga odio repellendus labore recusandae repudiandae unde cum,
          dolorum at iusto magnam nobis? Nobis aliquam velit eos repudiandae
          commodi?
        </b-card-text>
        <b-button variant="primary">Comprar</b-button>
      </b-card>
    </b-col>
  </div>
</template>

<script>
export default {
  data() {
    return {
      descricao: 'lorem ipsum dolor sit amet consectetur adipis'
    }
  },
  props: {
    nome: {
      type: String,
      required: true,
    }
  }
}
</script>
