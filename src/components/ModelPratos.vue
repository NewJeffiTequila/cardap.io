<template>
  <div>
      <form @submit="onSubmit">
        <b-form-group
          label="Arroz"
          label-for="name-input"
          invalid-feedback="A quantidade deve ser colocada"

        >
          <b-form-input
            id="name-input"
            min="0.00"
            required
            type="number"
          ></b-form-input>
        </b-form-group>
        <b-form-group
          label="Feijão"
          label-for="name-input"
          invalid-feedback="A quantidade deve ser colocada"

        >
          <b-form-input
            id="name-input"
            min="0.00"
            required
            type="number"
          ></b-form-input>
        </b-form-group>
        <b-form-group
          label="Carne"
          label-for="name-input"
          invalid-feedback="A quantidade deve ser colocada"

        >
          <b-form-input
            id="name-input"
            min="0.00"
            required
            type="number"
          ></b-form-input>
        </b-form-group>
        <b-button class="mt-2" type="submit" variant="success" block>Salvar Pedido</b-button>
        <b-button class="mt-3" variant="danger" block @click="hideModal">Cancelar</b-button>
      </form>
  </div>
</template>

<script>
export default {
    data(){
        return{
            form: {
            email: '',
            name: '',
            food: null,
            checked: []
        },
        }
    },
    methods: {

      hideModal() {
        this.$refs['modal-pratos'].hide()
      },
      enviarPedido() {
        console.log('eviado');
      },
      onSubmit(event) {
          console.log(this.form)
        event.preventDefault()
        alert(JSON.stringify(this.form))
      },
    }
}
</script>

<style>

</style>